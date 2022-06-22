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


$start->setDateTime('2017-04-15T12:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);


$end->setDateTime('2017-04-15T14:00:00');
$end->setTimeZone('Pacific Standard Time');


$location = new Location();
$requestRequestBody->setLocation($location);


$location->setDisplayName('Harry\'s Bar');

$attendeesArray = [];

$attendees1 = new Attendee();

$attendees1AdditionalData = [
"type" => 'required',
];
$attendees1->setAdditionalData($attendees1AdditionalData);

$attendeesArray []= $attendees1;
$requestRequestBody->setAttendees($attendeesArray);
$requestRequestBody->setAllowNewTimeProposals(True);
$requestRequestBody->setTransactionId('7E163156-7762-4BEB-A1C6-729EA81755A7');
$requestConfiguration = new EventsRequestBuilderPostRequestConfiguration();

$headers = [
"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->events()->post($requestRequestBody, $requestConfiguration);


```