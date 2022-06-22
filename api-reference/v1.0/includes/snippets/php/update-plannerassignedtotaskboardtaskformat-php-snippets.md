---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerAssignedToTaskBoardTaskFormat();



$orderHintsByAssignee = new PlannerOrderHintsByAssignee();
$requestRequestBody->setOrderHintsByAssignee($orderHintsByAssignee);


$orderHintsByAssigneeAdditionalData = [
	"aaa27244-1db4-476a-a5cb-004607466324" => '8566473P 957764Jk!',
];
$orderHintsByAssignee->setAdditionalData($orderHintsByAssigneeAdditionalData);

$requestConfiguration = new AssignedToTaskBoardFormatRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
"If-Match" => "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->planner()->tasksById('plannerTask-id')->assignedToTaskBoardFormat()->patch($requestRequestBody, $requestConfiguration);


```