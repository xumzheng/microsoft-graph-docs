---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TodoTask();



$dueDateTime = new DateTimeTimeZone();
$requestRequestBody->setDueDateTime($dueDateTime);


$dueDateTime->setDateTime('2020-07-25T16:00:00');
$dueDateTime->setTimeZone('Eastern Standard Time');

$result =  $graphClient->me()->todo()->listsById('todoTaskList-id')->tasksById('todoTask-id')->patch($requestRequestBody);


```