---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new FindMeetingTimesPostRequestBody();


$attendeesArray = [];

$attendeesattendees1 = new AttendeeBase();

$attendeesattendees1AdditionalData = [
	"type" => 'required',
];
$attendeesattendees1->setAdditionalData($attendeesattendees1AdditionalData);

$attendeesArray []= $attendeesattendees1;
$requestRequestBody->setAttendees($attendeesArray);

$locationConstraint = new LocationConstraint();
$requestRequestBody->setLocationConstraint($locationConstraint);


$locationConstraint->setIsRequired(False);
$locationConstraint->setSuggestLocation(False);
$locationsArray = [];

$locationslocations1 = new LocationConstraintItem();

$locationslocations1AdditionalData = [
"resolveAvailability" => False,
"displayName" => 'Conf room Hood',
];
$locationslocations1->setAdditionalData($locationslocations1AdditionalData);

$locationsArray []= $locationslocations1;
$locationConstraint->setLocations($locationsArray);


$timeConstraint = new TimeConstraint();
$requestRequestBody->setTimeConstraint($timeConstraint);


$timeConstraint->setActivityDomain(new ActivityDomain('work'));
$timeSlotsArray = [];

$timeSlotstimeSlots1 = new TimeSlot();


$start = new DateTimeTimeZone();
$timeSlotstimeSlots1->setStart($start);


$start->setDateTime('2019-04-16T09:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$timeSlotstimeSlots1->setEnd($end);


$end->setDateTime('2019-04-18T17:00:00');
$end->setTimeZone('Pacific Standard Time');


$timeSlotsArray []= $timeSlotstimeSlots1;
$timeConstraint->setTimeSlots($timeSlotsArray);

$requestRequestBody->setIsOrganizerOptional('false');
$requestRequestBody->setMeetingDuration('PT1H');
$requestRequestBody->setReturnSuggestionReasons('true');
$requestRequestBody->setMinimumAttendeePercentage('100');
$requestConfiguration = new FindMeetingTimesRequestBuilderPostRequestConfiguration();

$headers = [
"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->findMeetingTimes()->post($requestRequestBody, $requestConfiguration);


```