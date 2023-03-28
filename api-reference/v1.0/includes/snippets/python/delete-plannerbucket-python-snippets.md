---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PlannerBucketRequestBuilderDeleteRequestConfiguration();

$headers = [
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

$requestConfiguration.headers = $headers;


$graphServiceClient.planner().bucketsById('plannerBucket-id').delete($requestConfiguration);


```