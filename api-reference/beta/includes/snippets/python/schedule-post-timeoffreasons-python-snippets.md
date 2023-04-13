---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeOffReason()
request_body.displayName = 'Vacation'

request_body.IconType(TimeOffReasonIconType('plane'))

request_body.isActive = true




result = await client.teams_by_id('team-id').schedule.timeOffReasons.post(request_body = request_body)


```