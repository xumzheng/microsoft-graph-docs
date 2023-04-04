---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = PlannerPlanRequestBuilderDeleteRequestConfiguration();

headers = [
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

request_config.headers = headers;


await client.planner.plansById('plannerPlan-id').delete(request_config);


```