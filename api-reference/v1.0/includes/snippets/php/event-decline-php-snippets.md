---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DeclinePostRequestBody();


$requestRequestBody->setComment('I won\'t be able to make this week. How about next week?');
$requestRequestBody->setSendResponse(True);

$proposedNewTime = new TimeSlot();
$requestRequestBody->setProposedNewTime($proposedNewTime);



$start = new DateTimeTimeZone();
$proposedNewTime->setStart($start);


$start->setDateTime('2019-12-02T18:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$proposedNewTime->setEnd($end);


$end->setDateTime('2019-12-02T19:00:00');
$end->setTimeZone('Pacific Standard Time');


$result =  $graphClient->me()->eventsById('event-id')->decline()->post($requestRequestBody);


```