---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EvaluateClassificationResultsPostRequestBody();



$contentInfo = new ContentInfo();
$requestRequestBody->setContentInfo($contentInfo);


$contentInfo->setFormat(new ContentFormat('default'));
$contentInfo->setIdentifier(null);
$contentInfo->setState(new ContentState('rest'));
$contentInfoAdditionalData = [
	"@odata.type" => '#microsoft.graph.contentInfo',
	"format@odata.type" => '#microsoft.graph.contentFormat',
	"state@odata.type" => '#microsoft.graph.contentState',
];
$contentInfo->setAdditionalData($contentInfoAdditionalData);

$classificationResultsArray = [];

$classificationResultsclassificationResults1 = new ClassificationResult();

$classificationResultsclassificationResults1AdditionalData = [
"sensitiveTypeId" => 'cb353f78-2b72-4c3c-8827-92ebe4f69fdf',
"count" => 4,
"confidenceLevel" => 75,
];
$classificationResultsclassificationResults1->setAdditionalData($classificationResultsclassificationResults1AdditionalData);

$classificationResultsArray []= $classificationResultsclassificationResults1;
$requestRequestBody->setClassificationResults($classificationResultsArray);
$requestConfiguration = new EvaluateClassificationResultsRequestBuilderPostRequestConfiguration();

$headers = [
"User-Agent" => "ContosoLOBApp/1.0",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->informationProtection()->policy()->labels()->evaluateClassificationResults()->post($requestRequestBody, $requestConfiguration);


```