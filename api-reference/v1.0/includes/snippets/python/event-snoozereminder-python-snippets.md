---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SnoozeReminderPostRequestBody();
newReminderTime = DateTimeTimeZone();
newReminderTime.setDateTime('dateTime-value');

newReminderTime.setTimeZone('timeZone-value');


requestBody.setNewReminderTime($newReminderTime);


awaitclient.me().eventsById('event-id').snoozeReminder().post(requestBody);


```