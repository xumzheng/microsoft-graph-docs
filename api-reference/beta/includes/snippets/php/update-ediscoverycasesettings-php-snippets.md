---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryCaseSettings();



$redundancyDetection = new RedundancyDetectionSettings();
$requestRequestBody->setRedundancyDetection($redundancyDetection);


$redundancyDetectionAdditionalData = [
	"@odata.type" => 'microsoft.graph.security.redundancyDetectionSettings',
];
$redundancyDetection->setAdditionalData($redundancyDetectionAdditionalData);


$topicModeling = new TopicModelingSettings();
$requestRequestBody->setTopicModeling($topicModeling);


$topicModelingAdditionalData = [
"@odata.type" => 'microsoft.graph.security.topicModelingSettings',
];
$topicModeling->setAdditionalData($topicModelingAdditionalData);


$ocr = new OcrSettings();
$requestRequestBody->setOcr($ocr);


$ocrAdditionalData = [
"@odata.type" => 'microsoft.graph.security.ocrSettings',
];
$ocr->setAdditionalData($ocrAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.security.ediscoveryCaseSettings',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->settings()->patch($requestRequestBody);


```