---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = PlannerPlanRequestBuilderGetRequestConfiguration(
)


result = await client.planner.rosters_by_id('plannerRoster-id').plans_by_id('plannerPlan-id').get()


```