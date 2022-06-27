---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerTask();



$assignments = new PlannerAssignments();
$requestRequestBody->setAssignments($assignments);


$assignmentsAdditionalData = [
];
$assignments->setAdditionalData($assignmentsAdditionalData);


$appliedCategories = new PlannerAppliedCategories();
$requestRequestBody->setAppliedCategories($appliedCategories);


$appliedCategoriesAdditionalData = [
"category3" => True,
"category4" => False,
];
$appliedCategories->setAdditionalData($appliedCategoriesAdditionalData);

$requestConfiguration = new PlannerTaskRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->planner()->tasksById('plannerTask-id')->patch($requestRequestBody, $requestConfiguration);


```