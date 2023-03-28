---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PlannerPlanRequestBuilderDeleteRequestConfiguration();

$headers = [
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

$requestConfiguration.headers = $headers;


$graphServiceClient.planner().plansById('plannerPlan-id').delete($requestConfiguration);


```