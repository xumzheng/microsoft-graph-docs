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
$responseStatus->setTime(new DateTime("2016-10-19T10:37:00Z"));

$requestRequestBody->setRecurrence(null);
$requestRequestBody->setUid('iCalUId-value');
$requestRequestBody->setReminderMinutesBeforeStart(99);
$requestRequestBody->setIsOnlineMeeting(True);
$requestRequestBody->setOnlineMeetingProvider(new OnlineMeetingProviderType('teamsForBusiness'));
$requestRequestBody->setIsReminderOn(True);
$requestRequestBody->setHideAttendees(False);
$requestRequestBody->setCategories( [
'Red category',],
$result =  $graphClient->me()->eventsById('event-id')->patch($requestRequestBody);


```