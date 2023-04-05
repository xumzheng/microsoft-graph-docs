---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerRoster()
request_body.set@odatatype('#microsoft.graph.plannerRoster')



result = await client.planner_rosters.post(request_body)


```