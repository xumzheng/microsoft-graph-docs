---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EvaluateRemovalPostRequestBody();



$contentInfo = new ContentInfo();
$requestRequestBody->setContentInfo($contentInfo);


$contentInfo->setFormat(new ContentFormat('default'));
$contentInfo->setIdentifier(null);
$contentInfo->setState(new ContentState('rest'));
$metadataArray = [];

$metadata1 = new KeyValuePair();

$metadata1->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled');
$metadata1->setValue('True');
$metadata1AdditionalData = [
		"@odata.type" => '#microsoft.graph.keyValuePair',
	];
$metadata1->setAdditionalData($metadata1AdditionalData);

$metadataArray []= $metadata1;

$metadata2 = new KeyValuePair();

$metadata2->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method');
$metadata2->setValue('Standard');
$metadata2AdditionalData = [
	"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadata2->setAdditionalData($metadata2AdditionalData);

$metadataArray []= $metadata2;

$metadata3 = new KeyValuePair();

$metadata3->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate');
$metadata3->setValue('1/1/0001 12:00:00 AM');
$metadata3AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadata3->setAdditionalData($metadata3AdditionalData);

$metadataArray []= $metadata3;

$metadata4 = new KeyValuePair();

$metadata4->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId');
$metadata4->setValue('cfa4cf1d-a337-4481-aa99-19d8f3d63f7c');
$metadata4AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadata4->setAdditionalData($metadata4AdditionalData);

$metadataArray []= $metadata4;

$metadata5 = new KeyValuePair();

$metadata5->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name');
$metadata5->setValue('General');
$metadata5AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadata5->setAdditionalData($metadata5AdditionalData);

$metadataArray []= $metadata5;

$metadata6 = new KeyValuePair();

$metadata6->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits');
$metadata6->setValue('0');
$metadata6AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadata6->setAdditionalData($metadata6AdditionalData);

$metadataArray []= $metadata6;

$metadata7 = new KeyValuePair();

$metadata7->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId');
$metadata7->setValue('00000000-0000-0000-0000-000000000000');
$metadata7AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadata7->setAdditionalData($metadata7AdditionalData);

$metadataArray []= $metadata7;
$contentInfo->setMetadata($metadataArray);
$contentInfoAdditionalData = [
"@odata.type" => '#microsoft.graph.contentInfo',
"format@odata.type" => '#microsoft.graph.contentFormat',
"state@odata.type" => '#microsoft.graph.contentState',
"metadata@odata.type" => '#Collection(microsoft.graph.keyValuePair)',
];
$contentInfo->setAdditionalData($contentInfoAdditionalData);


$downgradeJustification = new DowngradeJustification();
$requestRequestBody->setDowngradeJustification($downgradeJustification);


$downgradeJustification->setJustificationMessage('The information has been declassified.');
$downgradeJustification->setIsDowngradeJustified(True);

$requestConfiguration = new EvaluateRemovalRequestBuilderPostRequestConfiguration();

$headers = [
"User-Agent" => "ContosoLOBApp/1.0",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->informationProtection()->policy()->labels()->evaluateRemoval()->post($requestRequestBody, $requestConfiguration);


```