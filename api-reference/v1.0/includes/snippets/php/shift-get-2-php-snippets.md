---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ShiftPreferences();


$requestRequestBody->setId('SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7');
$availabilityArray = [];

$availabilityavailability1 = new ShiftAvailability();


$recurrence = new PatternedRecurrence();
$availabilityavailability1->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('Weekly'));
$daysOfWeekArray = [];
'Monday',$daysOfWeekArray []= $daysOfWeekdaysOfWeek1;
'Wednesday',$daysOfWeekArray []= $daysOfWeekdaysOfWeek2;
'Friday',$daysOfWeekArray []= $daysOfWeekdaysOfWeek3;
$pattern->setDaysOfWeek($daysOfWeekArray);
$pattern->setInterval(1);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('noEnd'));


$availabilityavailability1->setTimeZone('Pacific Standard Time');
$availabilityavailability1->setTimeSlots(null);

$availabilityArray []= $availabilityavailability1;
$requestRequestBody->setAvailability($availabilityArray);
$requestRequestBodyAdditionalData = [
"@odata.etag" => '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->usersById('user-id')->settings()->shiftPreferences()->patch($requestRequestBody);


```