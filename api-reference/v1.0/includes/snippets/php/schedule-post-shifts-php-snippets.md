---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Shift();


$requestRequestBody->setId('SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8');
$requestRequestBody->setUserId('c5d0c76b-80c4-481c-be50-923cd8d680a1');
$requestRequestBody->setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0');

$sharedShift = new ShiftItem();
$requestRequestBody->setSharedShift($sharedShift);


$sharedShift->setDisplayName('Day shift');
$sharedShift->setNotes('Please do inventory as part of your shift.');
$sharedShift->setStartDateTime(new DateTime("2019-03-11T15:00:00Z"));
$sharedShift->setEndDateTime(new DateTime("2019-03-12T00:00:00Z"));
$sharedShift->setTheme(new ScheduleEntityTheme('blue'));
$activitiesArray = [];

$activities1 = new ShiftActivity();

$activities1->setIsPaid(True);
$activities1->setStartDateTime(new DateTime("2019-03-11T15:00:00Z"));
$activities1->setEndDateTime(new DateTime("2019-03-11T15:15:00Z"));
$activities1->setCode('');
$activities1->setDisplayName('Lunch');

$activitiesArray []= $activities1;
$sharedShift->setActivities($activitiesArray);


$draftShift = new ShiftItem();
$requestRequestBody->setDraftShift($draftShift);


$draftShift->setDisplayName('Day shift');
$draftShift->setNotes('Please do inventory as part of your shift.');
$draftShift->setStartDateTime(new DateTime("2019-03-11T15:00:00Z"));
$draftShift->setEndDateTime(new DateTime("2019-03-12T00:00:00Z"));
$draftShift->setTheme(new ScheduleEntityTheme('blue'));
$activitiesArray = [];

$activities1 = new ShiftActivity();

$activities1->setIsPaid(True);
$activities1->setStartDateTime(new DateTime("2019-03-11T15:00:00Z"));
$activities1->setEndDateTime(new DateTime("2019-03-11T15:30:00Z"));
$activities1->setCode('');
$activities1->setDisplayName('Lunch');

$activitiesArray []= $activities1;
$draftShift->setActivities($activitiesArray);

$result =  $graphClient->teamsById('team-id')->schedule()->shifts()->post($requestRequestBody);


```