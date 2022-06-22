---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewInstance();



$scope = new AccessReviewScope();
$requestRequestBody->setScope($scope);


$scopeAdditionalData = [
	"@odata.type" => '#microsoft.graph.principalResourceMembershipsScope',
	"principalScopes" =>  [
	],
	"resourceScopes" =>  [
	],
];
$scope->setAdditionalData($scopeAdditionalData);

$reviewersArray = [];

$reviewers1 = new AccessReviewReviewerScope();

$reviewers1AdditionalData = [
	"query" => '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
	"queryType" => 'MicrosoftGraph',
];
$reviewers1->setAdditionalData($reviewers1AdditionalData);

$reviewersArray []= $reviewers1;
$requestRequestBody->setReviewers($reviewersArray);
$fallbackReviewersArray = [];

$fallbackReviewers1 = new AccessReviewReviewerScope();

$fallbackReviewers1AdditionalData = [
"query" => '/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewers1->setAdditionalData($fallbackReviewers1AdditionalData);

$fallbackReviewersArray []= $fallbackReviewers1;

$fallbackReviewers2 = new AccessReviewReviewerScope();

$fallbackReviewers2AdditionalData = [
"query" => '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewers2->setAdditionalData($fallbackReviewers2AdditionalData);

$fallbackReviewersArray []= $fallbackReviewers2;
$requestRequestBody->setFallbackReviewers($fallbackReviewersArray);
$result =  $graphClient->identityGovernance()->accessReviews()->definitionsById('accessReviewScheduleDefinition-id')->instancesById('accessReviewInstance-id')->patch($requestRequestBody);


```