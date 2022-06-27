---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingAppointment();



$endDateTime = new DateTimeTimeZone();
$requestRequestBody->setEndDateTime($endDateTime);


$endDateTime->setDateTime('2018-05-06T12:30:00.0000000+00:00');
$endDateTime->setTimeZone('UTC');
$endDateTimeAdditionalData = [
	"@odata.type" => '#microsoft.graph.dateTimeTimeZone',
];
$endDateTime->setAdditionalData($endDateTimeAdditionalData);


$startDateTime = new DateTimeTimeZone();
$requestRequestBody->setStartDateTime($startDateTime);


$startDateTime->setDateTime('2018-05-06T12:00:00.0000000+00:00');
$startDateTime->setTimeZone('UTC');
$startDateTimeAdditionalData = [
"@odata.type" => '#microsoft.graph.dateTimeTimeZone',
];
$startDateTime->setAdditionalData($startDateTimeAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.bookingAppointment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->solutions()->bookingBusinessesById('bookingBusiness-id')->appointmentsById('bookingAppointment-id')->patch($requestRequestBody);


```