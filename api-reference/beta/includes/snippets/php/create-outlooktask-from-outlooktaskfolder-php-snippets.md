---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookTask();


$requestRequestBody->setSubject('Shop for dinner');

$startDateTime = new DateTimeTimeZone();
$requestRequestBody->setStartDateTime($startDateTime);


$startDateTime->setDateTime('2016-04-23T18:00:00');
$startDateTime->setTimeZone('Pacific Standard Time');


$dueDateTime = new DateTimeTimeZone();
$requestRequestBody->setDueDateTime($dueDateTime);


$dueDateTime->setDateTime('2016-04-25T13:00:00');
$dueDateTime->setTimeZone('Pacific Standard Time');

$result =  $graphClient->me()->outlook()->taskFoldersById('outlookTaskFolder-id')->tasks()->post($requestRequestBody);


```