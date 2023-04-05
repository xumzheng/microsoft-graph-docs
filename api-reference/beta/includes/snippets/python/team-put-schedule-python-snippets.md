---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schedule()
request_body.setEnabled(true)

request_body.setTimeZone('America/Chicago')



result = await client.teamsby_id('team-id')_schedule.put(request_body)


```