---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AdminConsentRequestPolicyPutRequestBody();


$requestRequestBodyAdditionalData = [
	"isEnabled" => True,
	"notifyReviewers" => True,
	"remindersEnabled" => True,
	"requestDurationInDays" => 5,
	"reviewers" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->adminConsentRequestPolicy()->put($requestRequestBody);


```