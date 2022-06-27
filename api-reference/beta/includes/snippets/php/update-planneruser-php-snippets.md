---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerUser();



$favoritePlanReferences = new PlannerFavoritePlanReferenceCollection();
$requestRequestBody->setFavoritePlanReferences($favoritePlanReferences);


$favoritePlanReferencesAdditionalData = [
	"7oTB5aMIAE2rVo-1N-L7RmQAGX2q" => null,
];
$favoritePlanReferences->setAdditionalData($favoritePlanReferencesAdditionalData);


$recentPlanReferences = new PlannerRecentPlanReferenceCollection();
$requestRequestBody->setRecentPlanReferences($recentPlanReferences);


$recentPlanReferencesAdditionalData = [
];
$recentPlanReferences->setAdditionalData($recentPlanReferencesAdditionalData);

$requestConfiguration = new PlannerRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->planner()->patch($requestRequestBody, $requestConfiguration);


```