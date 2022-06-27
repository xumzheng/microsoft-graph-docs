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

$speakersspeakers1 = new MeetingSpeaker();

$speakersspeakers1->setDisplayName('Henry Ross');
$speakersspeakers1->setBio('Chairman and Chief Executive Officer');

$speakersArray []= $speakersspeakers1;

$speakersspeakers2 = new MeetingSpeaker();

$speakersspeakers2->setDisplayName('Fred Ryan');
$speakersspeakers2->setBio('CVP');

$speakersArray []= $speakersspeakers2;
$requestRequestBody->setSpeakers($speakersArray);
$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->patch($requestRequestBody);


```