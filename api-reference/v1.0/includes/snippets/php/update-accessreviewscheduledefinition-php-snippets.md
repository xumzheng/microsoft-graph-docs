---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewScheduleDefinition-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => '60860cdd-fb4d-4054-91ba-f75e04444aa6',
	"displayName" => 'Test world UPDATED NAME!',
	"descriptionForAdmins" => 'Test world',
	"descriptionForReviewers" => 'Test world',
	"reviewers" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityGovernance()->accessReviews()->definitionsById('accessReviewScheduleDefinition-id')->put($requestRequestBody);


```