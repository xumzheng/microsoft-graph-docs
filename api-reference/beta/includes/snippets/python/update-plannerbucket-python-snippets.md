---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PlannerBucket();
$requestBody.setName('Development');


$requestConfiguration = new PlannerBucketRequestBuilderPatchRequestConfiguration();

$headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.planner().bucketsById('plannerBucket-id').patch($requestBody, $requestConfiguration);


```