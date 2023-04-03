---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SnoozeReminderPostRequestBody();
newReminderTime = DateTimeTimeZone();
newReminderTime.setDateTime('dateTime-value');

newReminderTime.setTimeZone('timeZone-value');


requestBody.setNewReminderTime($newReminderTime);


graphServiceClient.me().eventsById('event-id').snoozeReminder().post(requestBody);


```