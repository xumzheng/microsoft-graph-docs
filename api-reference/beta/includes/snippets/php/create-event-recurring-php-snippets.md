---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Event();


$requestRequestBody->setSubject('Let\'s go for lunch');

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('Does noon time work for you?');


$start = new DateTimeTimeZone();
$requestRequestBody->setStart($start);


$start->setDateTime('2017-09-04T12:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);


$end->setDateTime('2017-09-04T14:00:00');
$end->setTimeZone('Pacific Standard Time');


$recurrence = new PatternedRecurrence();
$requestRequestBody->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('weekly'));
$pattern->setInterval(1);
$daysOfWeekArray = [];
'Monday',$daysOfWeekArray []= $daysOfWeekdaysOfWeek1;
$pattern->setDaysOfWeek($daysOfWeekArray);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('endDate'));
$range->setStartDate(new Date("2017-09-04"));
$range->setEndDate(new Date("2017-12-31"));



$location = new Location();
$requestRequestBody->setLocation($location);


$location->setDisplayName('Harry\'s Bar');

$attendeesArray = [];

$attendeesattendees1 = new Attendee();

$attendeesattendees1AdditionalData = [
"type" => 'required',
];
$attendeesattendees1->setAdditionalData($attendeesattendees1AdditionalData);

$attendeesArray []= $attendeesattendees1;
$requestRequestBody->setAttendees($attendeesArray);
$result =  $graphClient->me()->events()->post($requestRequestBody);


```