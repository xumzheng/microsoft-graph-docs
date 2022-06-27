---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerPlanDetails();



$sharedWith = new PlannerUserIds();
$requestRequestBody->setSharedWith($sharedWith);


$sharedWithAdditionalData = [
	"6463a5ce-2119-4198-9f2a-628761df4a62" => True,
	"d95e6152-f683-4d78-9ff5-67ad180fea4a" => False,
];
$sharedWith->setAdditionalData($sharedWithAdditionalData);


$categoryDescriptions = new PlannerCategoryDescriptions();
$requestRequestBody->setCategoryDescriptions($categoryDescriptions);


$categoryDescriptions->setCategory1('Indoors');
$categoryDescriptions->setCategory3(null);

$requestConfiguration = new DetailsRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->planner()->plansById('plannerPlan-id')->details()->patch($requestRequestBody, $requestConfiguration);


```