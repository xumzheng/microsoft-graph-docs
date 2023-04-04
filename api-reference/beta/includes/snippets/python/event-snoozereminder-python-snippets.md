---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SnoozeReminderPostRequestBody();
newReminderTime = DateTimeTimeZone();
newReminderTime.setDateTime('2016-10-19T10:37:00Z');

newReminderTime.setTimeZone('timeZone-value');


request_body.setNewReminderTime($newReminderTime);


await client.me().eventsById('event-id').snoozeReminder().post(request_body);


```