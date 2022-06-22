---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GetSchedulePostRequestBody();


$requestRequestBody->setSchedules( [
'adelev@contoso.onmicrosoft.com','meganb@contoso.onmicrosoft.com',],

$startTime = new DateTimeTimeZone();
$requestRequestBody->setStartTime($startTime);


$startTime->setDateTime('2019-03-15T09:00:00');
$startTime->setTimeZone('Pacific Standard Time');


$endTime = new DateTimeTimeZone();
$requestRequestBody->setEndTime($endTime);


$endTime->setDateTime('2019-03-15T18:00:00');
$endTime->setTimeZone('Pacific Standard Time');

$requestRequestBody->setAvailabilityViewInterval(60);
$requestConfiguration = new GetScheduleRequestBuilderPostRequestConfiguration();

$headers = [
"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->calendar()->getSchedule()->post($requestRequestBody, $requestConfiguration);


```