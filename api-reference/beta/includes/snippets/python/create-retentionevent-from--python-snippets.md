---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RetentionEvent();
$requestBody->set@odatatype('#microsoft.graph.security.retentionEvent');

$requestBody->setDisplayName('String');

$requestBody->setDescription('String');

$eventQueriesEventQuery1 = new EventQuery();
$eventQueriesEventQuery1->set@odatatype('microsoft.graph.security.eventQueries');


$eventQueriesArray []= $eventQueriesEventQuery1;
$requestBody->setEventQueries($eventQueriesArray);


$requestBody->setEventTriggerDateTime(new DateTime('String (timestamp)'));

$createdBy = new IdentitySet();
$createdBy->set@odatatype('microsoft.graph.identitySet');


$requestBody->setCreatedBy($createdBy);
$eventPropagationResultsEventPropagationResult1 = new EventPropagationResult();
$eventPropagationResultsEventPropagationResult1->set@odatatype('microsoft.graph.security.eventPropagationResult');


$eventPropagationResultsArray []= $eventPropagationResultsEventPropagationResult1;
$requestBody->setEventPropagationResults($eventPropagationResultsArray);


$eventStatus = new RetentionEventStatus();
$eventStatus->set@odatatype('microsoft.graph.security.retentionEventStatus');


$requestBody->setEventStatus($eventStatus);
$requestBody->setLastStatusUpdateDateTime(new DateTime('String (timestamp)'));



$requestResult = $graphServiceClient->security()->triggers()->retentionEvents()->post($requestBody);


```