---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OutlookTask();
$requestBody->setSubject('Shop for dinner');

$startDateTime = new DateTimeTimeZone();
$startDateTime->setDateTime('2016-04-23T18:00:00');

$startDateTime->setTimeZone('Pacific Standard Time');


$requestBody->setStartDateTime($startDateTime);
$dueDateTime = new DateTimeTimeZone();
$dueDateTime->setDateTime('2016-04-25T13:00:00');

$dueDateTime->setTimeZone('Pacific Standard Time');


$requestBody->setDueDateTime($dueDateTime);


$requestResult = $graphServiceClient->me()->outlook()->taskFoldersById('outlookTaskFolder-id')->tasks()->post($requestBody);


```