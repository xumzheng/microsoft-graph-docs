---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookTask();


$requestRequestBody->setSubject('Shop for children\'s weekend');

$startDateTime = new DateTimeTimeZone();
$requestRequestBody->setStartDateTime($startDateTime);


$startDateTime->setDateTime('2016-05-03T09:00:00');
$startDateTime->setTimeZone('Eastern Standard Time');


$dueDateTime = new DateTimeTimeZone();
$requestRequestBody->setDueDateTime($dueDateTime);


$dueDateTime->setDateTime('2016-05-05T16:00:00');
$dueDateTime->setTimeZone('Eastern Standard Time');

$requestConfiguration = new TasksRequestBuilderPostRequestConfiguration();

$headers = [
"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->outlook()->tasks()->post($requestRequestBody, $requestConfiguration);


```