---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OpenShift();


$requestRequestBody->setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0');

$sharedOpenShift = new OpenShiftItem();
$requestRequestBody->setSharedOpenShift($sharedOpenShift);


$sharedOpenShift->setNotes('Inventory Management');
$sharedOpenShift->setOpenSlotCount(5);
$sharedOpenShift->setDisplayName('Field shift');
$sharedOpenShift->setStartDateTime(new DateTime("2018-10-04T00:58:45.340Z"));
$sharedOpenShift->setEndDateTime(new DateTime("2018-10-04T09:50:45.332Z"));
$sharedOpenShift->setTheme(new ScheduleEntityTheme('white'));
$activitiesArray = [];

$activities1 = new ShiftActivity();

$activities1->setIsPaid(True);
$activities1->setStartDateTime(new DateTime("2018-10-04T00:58:45.340Z"));
$activities1->setEndDateTime(new DateTime("2018-10-04T01:58:45.340Z"));
$activities1->setCode('');
$activities1->setDisplayName('Lunch');

$activitiesArray []= $activities1;
$sharedOpenShift->setActivities($activitiesArray);

$requestRequestBody->setDraftOpenShift(null);
$result =  $graphClient->teamsById('team-id')->schedule()->openShiftsById('openShift-id')->patch($requestRequestBody);


```