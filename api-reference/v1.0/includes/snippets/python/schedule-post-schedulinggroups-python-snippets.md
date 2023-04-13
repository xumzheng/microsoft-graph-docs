---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchedulingGroup()
request_body.displayName = 'Cashiers'

request_body.is_active = True

request_body.UserIds(['c5d0c76b-80c4-481c-be50-923cd8d680a1', '2a4296b3-a28a-44ba-bc66-0274b9b95851', ])




result = await client.teams_by_id('team-id').schedule.schedulingGroups.post(request_body = request_body)


```