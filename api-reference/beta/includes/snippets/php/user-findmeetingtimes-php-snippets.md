---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new FindMeetingTimesPostRequestBody();


$attendeesArray = [];

$attendees1 = new AttendeeBase();

$attendees1AdditionalData = [
		"type" => 'required',
	];
$attendees1->setAdditionalData($attendees1AdditionalData);

$attendeesArray []= $attendees1;
$requestRequestBody->setAttendees($attendeesArray);

$locationConstraint = new LocationConstraint();
$requestRequestBody->setLocationConstraint($locationConstraint);


$locationConstraint->setIsRequired('false');
$locationConstraint->setSuggestLocation('false');
$locationsArray = [];

$locations1 = new LocationConstraintItem();

$locations1AdditionalData = [
	"resolveAvailability" => 'false',
	"displayName" => 'Conf room Hood',
];
$locations1->setAdditionalData($locations1AdditionalData);

$locationsArray []= $locations1;
$locationConstraint->setLocations($locationsArray);


$timeConstraint = new TimeConstraint();
$requestRequestBody->setTimeConstraint($timeConstraint);


$timeConstraint->setActivityDomain(new ActivityDomain('work'));
$timeSlotsArray = [];

$timeSlots1 = new TimeSlot();


$start = new DateTimeTimeZone();
$timeSlots1->setStart($start);


$start->setDateTime('2019-04-16T09:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$timeSlots1->setEnd($end);


$end->setDateTime('2019-04-18T17:00:00');
$end->setTimeZone('Pacific Standard Time');


$timeSlotsArray []= $timeSlots1;
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