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

responseStatus.time = DateTime('2016-10-19T10:37:00Z')


request_body.response_status = responseStatus
request_body.recurrence=null

request_body.uid = 'iCalUId-value'

request_body.reminder_minutes_before_start = 99

request_body.is_online_meeting = True

request_body.OnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))

request_body.is_reminder_on = True

request_body.hide_attendees = False

request_body.Categories(['Red category', ])




result = await client.me.events_by_id('event-id').patch(request_body = request_body)


```