---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EvaluateApplicationPostRequestBody();



$contentInfo = new ContentInfo();
$requestRequestBody->setContentInfo($contentInfo);


$contentInfo->setFormat(new ContentFormat('default'));
$contentInfo->setIdentifier(null);
$contentInfo->setState(new ContentState('rest'));
$metadataArray = [];

$metadatametadata1 = new KeyValuePair();

$metadatametadata1->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled');
$metadatametadata1->setValue('True');
$metadatametadata1AdditionalData = [
	"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata1->setAdditionalData($metadatametadata1AdditionalData);

$metadataArray []= $metadatametadata1;

$metadatametadata2 = new KeyValuePair();

$metadatametadata2->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method');
$metadatametadata2->setValue('Standard');
$metadatametadata2AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata2->setAdditionalData($metadatametadata2AdditionalData);

$metadataArray []= $metadatametadata2;

$metadatametadata3 = new KeyValuePair();

$metadatametadata3->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate');
$metadatametadata3->setValue('1/1/0001 12:00:00 AM');
$metadatametadata3AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata3->setAdditionalData($metadatametadata3AdditionalData);

$metadataArray []= $metadatametadata3;

$metadatametadata4 = new KeyValuePair();

$metadatametadata4->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId');
$metadatametadata4->setValue('cfa4cf1d-a337-4481-aa99-19d8f3d63f7c');
$metadatametadata4AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata4->setAdditionalData($metadatametadata4AdditionalData);

$metadataArray []= $metadatametadata4;

$metadatametadata5 = new KeyValuePair();

$metadatametadata5->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name');
$metadatametadata5->setValue('General');
$metadatametadata5AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata5->setAdditionalData($metadatametadata5AdditionalData);

$metadataArray []= $metadatametadata5;

$metadatametadata6 = new KeyValuePair();

$metadatametadata6->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits');
$metadatametadata6->setValue('0');
$metadatametadata6AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata6->setAdditionalData($metadatametadata6AdditionalData);

$metadataArray []= $metadatametadata6;

$metadatametadata7 = new KeyValuePair();

$metadatametadata7->setName('MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId');
$metadatametadata7->setValue('00000000-0000-0000-0000-000000000000');
$metadatametadata7AdditionalData = [
"@odata.type" => '#microsoft.graph.keyValuePair',
];
$metadatametadata7->setAdditionalData($metadatametadata7AdditionalData);

$metadataArray []= $metadatametadata7;
$contentInfo->setMetadata($metadataArray);
$contentInfoAdditionalData = [
"@odata.type" => '#microsoft.graph.contentInfo',
"format@odata.type" => '#microsoft.graph.contentFormat',
"state@odata.type" => '#microsoft.graph.contentState',
"metadata@odata.type" => '#Collection(microsoft.graph.keyValuePair)',
];
$contentInfo->setAdditionalData($contentInfoAdditionalData);


$labelingOptions = new LabelingOptions();
$requestRequestBody->setLabelingOptions($labelingOptions);


$labelingOptions->setAssignmentMethod(new AssignmentMethod('standard'));
$labelingOptions->setLabelId('97309856-9c28-4ac6-9382-5f8bc20c457b');
$labelingOptions->setDowngradeJustification(null);
$extendedPropertiesArray = [];
$labelingOptions->setExtendedProperties($extendedPropertiesArray);
$labelingOptionsAdditionalData = [
"@odata.type" => '#microsoft.graph.labelingOptions',
"assignmentMethod@odata.type" => '#microsoft.graph.assignmentMethod',
"labelId@odata.type" => '#Guid',
"extendedProperties@odata.type" => '#Collection(microsoft.graph.keyValuePair)',
];
$labelingOptions->setAdditionalData($labelingOptionsAdditionalData);

$requestConfiguration = new EvaluateApplicationRequestBuilderPostRequestConfiguration();

$headers = [
"User-Agent" => "ContosoLOBApp/1.0",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->informationProtection()->policy()->labels()->evaluateApplication()->post($requestRequestBody, $requestConfiguration);


```