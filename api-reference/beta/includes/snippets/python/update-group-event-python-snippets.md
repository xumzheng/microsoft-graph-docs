---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.originalStartTimeZone = 'originalStartTimeZone-value'

request_body.originalEndTimeZone = 'originalEndTimeZone-value'

response_status = ResponseStatus()
responseStatus.Response(ResponseType('none'))

responseStatus.time = DateTime('datetime-value')


request_body.response_status = responseStatus
request_body.uid = 'iCalUId-value'

request_body.reminder_minutes_before_start = 99

request_body.is_reminder_on = True




result = await client.groups_by_id('group-id').events_by_id('event-id').patch(request_body = request_body)


```