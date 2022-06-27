---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerBucketTaskBoardTaskFormat();


$requestRequestBody->setOrderHint('A6673H Ejkl!');
$requestConfiguration = new BucketTaskBoardFormatRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->planner()->tasksById('plannerTask-id')->bucketTaskBoardFormat()->patch($requestRequestBody, $requestConfiguration);


```