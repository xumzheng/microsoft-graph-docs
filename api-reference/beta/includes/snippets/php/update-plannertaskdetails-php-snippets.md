---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerTaskDetails();


$requestRequestBody->setPreviewType(new PlannerPreviewType('noPreview'));

$references = new PlannerExternalReferences();
$requestRequestBody->setReferences($references);


$referencesAdditionalData = [
	"http%3A//www%2Ebing%2Ecom" => null,
];
$references->setAdditionalData($referencesAdditionalData);


$checklist = new PlannerChecklistItems();
$requestRequestBody->setChecklist($checklist);


$checklistAdditionalData = [
"a93c93c5-10a6-4167-9551-8bafa09967a7" => null,
];
$checklist->setAdditionalData($checklistAdditionalData);

$requestConfiguration = new DetailsRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->planner()->tasksById('plannerTask-id')->details()->patch($requestRequestBody, $requestConfiguration);


```