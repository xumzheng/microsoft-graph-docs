---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OpenShift();


$requestRequestBody->setId('OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8');
$requestRequestBody->setSchedulingGroupId('TAG_228940ed-ff84-4e25-b129-1b395cf78be0');

$sharedOpenShift = new OpenShiftItem();
$requestRequestBody->setSharedOpenShift($sharedOpenShift);


$sharedOpenShift->setNotes('InventoryManagement');
$sharedOpenShift->setOpenSlotCount(2);
$sharedOpenShift->setDisplayName('Dayshift');
$sharedOpenShift->setStartDateTime(new DateTime("2018-10-04T00: 58: 45.340Z"));
$sharedOpenShift->setEndDateTime(new DateTime("2018-10-04T09: 50: 45.332Z"));
$sharedOpenShift->setTheme(new ScheduleEntityTheme('white'));
$activitiesArray = [];

$activitiesactivities1 = new ShiftActivity();

$activitiesactivities1->setIsPaid(True);
$activitiesactivities1->setStartDateTime(new DateTime("2018-10-04T00: 58: 45.340Z"));
$activitiesactivities1->setEndDateTime(new DateTime("2018-10-04T01: 58: 45.340Z"));
$activitiesactivities1->setCode('');
$activitiesactivities1->setDisplayName('Lunch');

$activitiesArray []= $activitiesactivities1;
$sharedOpenShift->setActivities($activitiesArray);

$requestRequestBody->setDraftOpenShift(null);
$requestRequestBody->setCreatedDateTime(new DateTime("2019-03-14T04: 32: 51.451Z"));
$requestRequestBody->setLastModifiedDateTime(new DateTime("2019-03-14T05: 32: 51.451Z"));

$lastModifiedBy = new IdentitySet();
$requestRequestBody->setLastModifiedBy($lastModifiedBy);


$lastModifiedBy->setApplication(null);
$lastModifiedBy->setDevice(null);

$user = new Identity();
$lastModifiedBy->setUser($user);


$user->setId('366c0b19-49b1-41b5-a03f-9f3887bd0ed8');
$user->setDisplayName('JohnDoe');

$lastModifiedByAdditionalData = [
"conversation" => null,
];
$lastModifiedBy->setAdditionalData($lastModifiedByAdditionalData);

$requestConfiguration = new OpenShiftsRequestBuilderPostRequestConfiguration();

$headers = [
"Authorization" => "Bearer {token}",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->openShifts()->post($requestRequestBody, $requestConfiguration);


```