---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerRosterMember()
request_body.set@odatatype('#microsoft.graph.plannerRosterMember')

request_body.setUserId('String')



result = await client.planner.rosters._by_id('plannerRoster-id').members.post(request_body)


```