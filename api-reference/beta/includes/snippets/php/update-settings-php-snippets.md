---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CaseSettings();



$redundancyDetection = new RedundancyDetectionSettings();
$requestRequestBody->setRedundancyDetection($redundancyDetection);


$redundancyDetection->setIsEnabled(False);
$redundancyDetection->setSimilarityThreshold(70);
$redundancyDetection->setMinWords(12);
$redundancyDetection->setMaxWords(400000);


$topicModeling = new TopicModelingSettings();
$requestRequestBody->setTopicModeling($topicModeling);


$topicModeling->setIsEnabled(False);
$topicModeling->setIgnoreNumbers(False);
$topicModeling->setTopicCount(50);
$topicModeling->setDynamicallyAdjustTopicCount(False);


$ocr = new OcrSettings();
$requestRequestBody->setOcr($ocr);


$ocr->setIsEnabled(True);
$ocr->setMaxImageSize(12000);

$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->settings()->patch($requestRequestBody);


```