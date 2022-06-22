---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MeetingRegistration();


$requestRequestBody->setSubject('Microsoft Ignite: Day 1');
$requestRequestBody->setStartDateTime(new DateTime("2021-11-02T08:00:00-08:00"));
$requestRequestBody->setEndDateTime(new DateTime("2021-11-02T15:45:00-08:00"));
$speakersArray = [];

$speakers1 = new MeetingSpeaker();

$speakers1->setDisplayName('Henry Ross');
$speakers1->setBio('Chairman and Chief Executive Officer');

$speakersArray []= $speakers1;

$speakers2 = new MeetingSpeaker();

$speakers2->setDisplayName('Fred Ryan');
$speakers2->setBio('CVP');

$speakersArray []= $speakers2;
$requestRequestBody->setSpeakers($speakersArray);
$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->patch($requestRequestBody);


```