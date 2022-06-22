---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingAppointment();



$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);


$end->setDateTime('2018-05-06T12:30:00.0000000+00:00');
$end->setTimeZone('UTC');
$endAdditionalData = [
	"@odata.type" => '#microsoft.graph.dateTimeTimeZone',
];
$end->setAdditionalData($endAdditionalData);


$invoiceDate = new DateTimeTimeZone();
$requestRequestBody->setInvoiceDate($invoiceDate);


$invoiceDate->setDateTime('2018-05-06T12:30:00.0000000+00:00');
$invoiceDate->setTimeZone('UTC');
$invoiceDateAdditionalData = [
"@odata.type" => '#microsoft.graph.dateTimeTimeZone',
];
$invoiceDate->setAdditionalData($invoiceDateAdditionalData);


$start = new DateTimeTimeZone();
$requestRequestBody->setStart($start);


$start->setDateTime('2018-05-06T12:00:00.0000000+00:00');
$start->setTimeZone('UTC');
$startAdditionalData = [
"@odata.type" => '#microsoft.graph.dateTimeTimeZone',
];
$start->setAdditionalData($startAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.bookingAppointment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->appointmentsById('bookingAppointment-id')->patch($requestRequestBody);


```