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
	"@odata.type" => '#microsoft.graph.emailFileAssessmentRequest',
	"recipientEmail" => 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com',
	"contentData" => 'UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->informationProtection()->threatAssessmentRequests()->post($requestRequestBody);


```