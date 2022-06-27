---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CreateOrGetPostRequestBody();



$chatInfo = new ChatInfo();
$requestRequestBody->setChatInfo($chatInfo);


$chatInfo->setThreadId('19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2');

$requestRequestBody->setStartDateTime(new DateTime("2020-02-06T01:49:21.3524945+00:00"));
$requestRequestBody->setEndDateTime(new DateTime("2020-02-06T02:19:21.3524945+00:00"));
$requestRequestBody->setExternalId('7eb8263f-d0e0-4149-bb1c-1f0476083c56');

$participants = new MeetingParticipants();
$requestRequestBody->setParticipants($participants);


$attendeesArray = [];

$attendeesattendees1 = new MeetingParticipantInfo();


$identity = new IdentitySet();
$attendeesattendees1->setIdentity($identity);



$user = new Identity();
$identity->setUser($user);


$user->setId('1f35f2e6-9cab-44ad-8d5a-b74c14720000');


$attendeesattendees1->setUpn('test1@contoso.com');

$attendeesArray []= $attendeesattendees1;
$participants->setAttendees($attendeesArray);

$requestRequestBody->setSubject('Create a meeting with customId provided');
$result =  $graphClient->me()->onlineMeetings()->createOrGet()->post($requestRequestBody);


```