---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookTask();



$dueDateTime = new DateTimeTimeZone();
$requestRequestBody->setDueDateTime($dueDateTime);


$dueDateTime->setDateTime('2016-05-06T16:00:00');
$dueDateTime->setTimeZone('Eastern Standard Time');

$requestConfiguration = new OutlookTaskRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "outlook.timezone=\"Eastern Standard Time\"",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->outlook()->tasksById('outlookTask-id')->patch($requestRequestBody, $requestConfiguration);


```