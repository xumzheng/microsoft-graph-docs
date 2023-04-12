---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schedule()
request_body.enabled = true

request_body.timeZone = 'America/Chicago'




result = await client.teams_by_id('team-id').schedule.put(request_body = request_body)


```