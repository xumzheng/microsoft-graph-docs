---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ThreatAssessmentRequest();


$requestRequestBody->setExpectedAssessment(new ThreatExpectedAssessment('block'));
$requestRequestBody->setCategory(new ThreatCategory('malware'));
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.fileAssessmentRequest',
	"fileName" => 'test.txt',
	"contentData" => 'VGhpcyBpcyBhIHRlc3QgZmlsZQ==',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->informationProtection()->threatAssessmentRequests()->post($requestRequestBody);


```