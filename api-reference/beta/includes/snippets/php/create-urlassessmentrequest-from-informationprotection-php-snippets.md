---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ThreatAssessmentRequest();


$requestRequestBody->setExpectedAssessment(new ThreatExpectedAssessment('block'));
$requestRequestBody->setCategory(new ThreatCategory('phishing'));
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.urlAssessmentRequest',
	"url" => 'http://test.com',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->informationProtection()->threatAssessmentRequests()->post($requestRequestBody);


```