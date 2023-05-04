---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Planner_roster_member()
request_body.@odata_type = '#microsoft.graph.plannerRosterMember'

request_body.user_id = 'String'




result = await client.planner.rosters.by_roster_id('plannerRoster-id').members.post(request_body = request_body)


```