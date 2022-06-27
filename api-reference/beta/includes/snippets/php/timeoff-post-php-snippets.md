---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TimeOff();


$requestRequestBody->setUserId('c5d0c76b-80c4-481c-be50-923cd8d680a1');

$sharedTimeOff = new TimeOffItem();
$requestRequestBody->setSharedTimeOff($sharedTimeOff);


$sharedTimeOff->setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7');
$sharedTimeOff->setStartDateTime(new DateTime("2019-03-11T07:00:00Z"));
$sharedTimeOff->setEndDateTime(new DateTime("2019-03-12T07:00:00Z"));
$sharedTimeOff->setTheme(new ScheduleEntityTheme('white'));


$draftTimeOff = new TimeOffItem();
$requestRequestBody->setDraftTimeOff($draftTimeOff);


$draftTimeOff->setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7');
$draftTimeOff->setStartDateTime(new DateTime("2019-03-11T07:00:00Z"));
$draftTimeOff->setEndDateTime(new DateTime("2019-03-12T07:00:00Z"));
$draftTimeOff->setTheme(new ScheduleEntityTheme('pink'));

$result =  $graphClient->teamsById('team-id')->schedule()->timesOff()->post($requestRequestBody);


```