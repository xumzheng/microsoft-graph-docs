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
	"principalScopes" => [],
"resourceScopes" => [],
];
$scope->setAdditionalData($scopeAdditionalData);

$reviewersArray = [];

$reviewersreviewers1 = new AccessReviewReviewerScope();

$reviewersreviewers1AdditionalData = [
"query" => '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
"queryType" => 'MicrosoftGraph',
];
$reviewersreviewers1->setAdditionalData($reviewersreviewers1AdditionalData);

$reviewersArray []= $reviewersreviewers1;
$requestRequestBody->setReviewers($reviewersArray);
$fallbackReviewersArray = [];

$fallbackReviewersfallbackReviewers1 = new AccessReviewReviewerScope();

$fallbackReviewersfallbackReviewers1AdditionalData = [
"query" => '/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewersfallbackReviewers1->setAdditionalData($fallbackReviewersfallbackReviewers1AdditionalData);

$fallbackReviewersArray []= $fallbackReviewersfallbackReviewers1;

$fallbackReviewersfallbackReviewers2 = new AccessReviewReviewerScope();

$fallbackReviewersfallbackReviewers2AdditionalData = [
"query" => '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewersfallbackReviewers2->setAdditionalData($fallbackReviewersfallbackReviewers2AdditionalData);

$fallbackReviewersArray []= $fallbackReviewersfallbackReviewers2;
$requestRequestBody->setFallbackReviewers($fallbackReviewersArray);
$result =  $graphClient->identityGovernance()->accessReviews()->definitionsById('accessReviewScheduleDefinition-id')->instancesById('accessReviewInstance-id')->patch($requestRequestBody);


```