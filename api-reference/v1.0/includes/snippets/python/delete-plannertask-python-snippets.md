---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PlannerTaskRequestBuilderDeleteRequestConfiguration();

$headers = [
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

$requestConfiguration.headers = $headers;


$graphServiceClient.planner().tasksById('plannerTask-id').delete($requestConfiguration);


```