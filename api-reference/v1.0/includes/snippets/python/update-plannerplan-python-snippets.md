---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerPlan()
request_body.setTitle('title-value')


request_config = PlannerPlanRequestBuilderPatchRequestConfiguration(
request_config = PlannerPlanRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"
headers['If-Match'] = "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""


result = await client.planner.plans_by_id('plannerPlan-id').patch(request_body, request_config, headers=request_config)


```