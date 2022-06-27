---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerPlan();


$requestRequestBody->setTitle('title-value');
$requestConfiguration = new PlannerPlanRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->planner()->plansById('plannerPlan-id')->patch($requestRequestBody, $requestConfiguration);


```