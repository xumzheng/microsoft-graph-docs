---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Event();


$requestRequestBody->setOriginalStartTimeZone('originalStartTimeZone-value');
$requestRequestBody->setOriginalEndTimeZone('originalEndTimeZone-value');

$responseStatus = new ResponseStatus();
$requestRequestBody->setResponseStatus($responseStatus);


$responseStatus->setResponse(new ResponseType(''));
$responseStatus->setTime(new DateTime("datetime-value"));

$requestRequestBody->setUid('iCalUId-value');
$requestRequestBody->setReminderMinutesBeforeStart(99);
$requestRequestBody->setIsReminderOn(True);
$result =  $graphClient->groupsById('group-id')->eventsById('event-id')->patch($requestRequestBody);


```