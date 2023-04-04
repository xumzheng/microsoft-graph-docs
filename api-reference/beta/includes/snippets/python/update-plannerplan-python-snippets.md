---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PlannerPlan();
request_body.setTitle('title-value');


request_config = PlannerPlanRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

request_config.headers = headers;


result = await client.planner.plansById('plannerPlan-id').patch(request_body, request_config);


```