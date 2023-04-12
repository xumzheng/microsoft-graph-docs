---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SnoozeReminderPostRequestBody()
newReminderTime = DateTimeTimeZone()
newReminderTime.dateTime = '2016-10-19T10:37:00Z'

newReminderTime.timeZone = 'timeZone-value'


request_body.newReminderTime = newReminderTime



await client.me.events_by_id('event-id').snoozeReminder.post(request_body = request_body)


```