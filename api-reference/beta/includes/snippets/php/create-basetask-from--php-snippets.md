---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BaseTask();


$requestRequestBody->setTextBody('String');
$requestRequestBody->setBodyLastModifiedDateTime(new DateTime("String (timestamp)"));
$requestRequestBody->setCompletedDateTime(new DateTime("String (timestamp)"));

$dueDateTime = new DateTimeTimeZone();
$requestRequestBody->setDueDateTime($dueDateTime);


$dueDateTimeAdditionalData = [
	"@odata.type" => 'microsoft.graph.dateTimeTimeZone',
];
$dueDateTime->setAdditionalData($dueDateTimeAdditionalData);


$startDateTime = new DateTimeTimeZone();
$requestRequestBody->setStartDateTime($startDateTime);


$startDateTimeAdditionalData = [
"@odata.type" => 'microsoft.graph.dateTimeTimeZone',
];
$startDateTime->setAdditionalData($startDateTimeAdditionalData);

$requestRequestBody->setImportance(new Importance('String'));

$recurrence = new PatternedRecurrence();
$requestRequestBody->setRecurrence($recurrence);


$recurrenceAdditionalData = [
"@odata.type" => 'microsoft.graph.patternedRecurrence',
];
$recurrence->setAdditionalData($recurrenceAdditionalData);

$requestRequestBody->setDisplayName('String');
$requestRequestBody->setStatus(new TaskStatus_v2('String'));

$viewpoint = new TaskViewpoint();
$requestRequestBody->setViewpoint($viewpoint);


$viewpointAdditionalData = [
"@odata.type" => 'microsoft.graph.taskViewpoint',
];
$viewpoint->setAdditionalData($viewpointAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.task',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->tasks()->listsById('baseTaskList-id')->tasks()->post($requestRequestBody);


```