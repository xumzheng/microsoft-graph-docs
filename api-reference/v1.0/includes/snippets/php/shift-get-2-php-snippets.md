---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ShiftPreferences();


$requestRequestBody->setId('SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7');
$availabilityArray = [];

$availability1 = new ShiftAvailability();


$recurrence = new PatternedRecurrence();
$availability1->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('Weekly'));
$daysOfWeekArray = [];
'Monday',$daysOfWeekArray []= $daysOfWeek1;
'Wednesday',$daysOfWeekArray []= $daysOfWeek2;
'Friday',$daysOfWeekArray []= $daysOfWeek3;
$pattern->setDaysOfWeek($daysOfWeekArray);
$pattern->setInterval(1);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('noEnd'));


$availability1->setTimeZone('Pacific Standard Time');
$availability1->setTimeSlots(null);

$availabilityArray []= $availability1;
$requestRequestBody->setAvailability($availabilityArray);
$requestRequestBodyAdditionalData = [
"@odata.etag" => '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->usersById('user-id')->settings()->shiftPreferences()->patch($requestRequestBody);


```