---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ThreatAssessmentRequest();


$requestRequestBody->setExpectedAssessment(new ThreatExpectedAssessment('block'));
$requestRequestBody->setCategory(new ThreatCategory('spam'));
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.mailAssessmentRequest',
	"recipientEmail" => 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com',
	"messageUri" => 'https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->informationProtection()->threatAssessmentRequests()->post($requestRequestBody);


```