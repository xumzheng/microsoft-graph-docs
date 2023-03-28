---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SnoozeReminderPostRequestBody();
$newReminderTime = new DateTimeTimeZone();
$newReminderTime->setDateTime('dateTime-value');

$newReminderTime->setTimeZone('timeZone-value');


$requestBody->setNewReminderTime($newReminderTime);


$graphServiceClient->me()->eventsById('event-id')->snoozeReminder()->post($requestBody);


```