---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SharePostRequestBody()
request_body.setNotifyTeam(true)

request_body.setStartDateTime(DateTime('2018-10-08T00:00:00.000Z'))

request_body.setEndDateTime(DateTime('2018-10-15T00:00:00.000Z'))



await client.teamsby_id('team-id').schedule.share.post(request_body)


```