---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SnoozeReminderPostRequestBody()
newReminderTime = DateTimeTimeZone()
newReminderTime.dateTime = 'dateTime-value'

newReminderTime.timeZone = 'timeZone-value'


request_body.newReminderTime = newReminderTime


request_configuration = SnoozeReminderRequestBuilderPostRequestConfiguration(
)


await client.me.events_by_id('event-id').snoozeReminder.post(request_body = request_body)


```