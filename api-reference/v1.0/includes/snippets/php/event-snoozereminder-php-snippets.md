---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NewReminderTimeRequestBody();



$newReminderTime = new DateTimeTimeZone();
$requestRequestBody->setNewReminderTime($newReminderTime);


$newReminderTime->setDateTime('dateTime-value');
$newReminderTime->setTimeZone('timeZone-value');

$result =  $graphClient->me()->eventsById('event-id')->snoozeReminder()->post($requestRequestBody);


```