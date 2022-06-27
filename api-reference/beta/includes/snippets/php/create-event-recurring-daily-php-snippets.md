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
$body->setContent('Does noon work for you?');


$start = new DateTimeTimeZone();
$requestRequestBody->setStart($start);


$start->setDateTime('2020-02-25T12:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);


$end->setDateTime('2020-02-25T14:00:00');
$end->setTimeZone('Pacific Standard Time');


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

$recurrence = new PatternedRecurrence();
$requestRequestBody->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('daily'));
$pattern->setInterval(1);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('numbered'));
$range->setStartDate(new Date("2020-02-25"));
$range->setNumberOfOccurrences(2);


$requestConfiguration = new EventsRequestBuilderPostRequestConfiguration();

$headers = [
"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->events()->post($requestRequestBody, $requestConfiguration);


```