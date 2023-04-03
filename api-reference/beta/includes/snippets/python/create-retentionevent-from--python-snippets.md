---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RetentionEvent();
requestBody.set@odatatype('#microsoft.graph.security.retentionEvent');

requestBody.setDisplayName('String');

requestBody.setDescription('String');

eventQueriesEventQuery1 = EventQuery();
eventQueriesEventQuery1.set@odatatype('microsoft.graph.security.eventQueries');


eventQueriesArray []= eventQueriesEventQuery1;
requestBody.setEventQueries(eventQueriesArray);


requestBody.setEventTriggerDateTime(DateTime('String (timestamp)'));

createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


requestBody.setCreatedBy($createdBy);
eventPropagationResultsEventPropagationResult1 = EventPropagationResult();
eventPropagationResultsEventPropagationResult1.set@odatatype('microsoft.graph.security.eventPropagationResult');


eventPropagationResultsArray []= eventPropagationResultsEventPropagationResult1;
requestBody.setEventPropagationResults(eventPropagationResultsArray);


eventStatus = RetentionEventStatus();
eventStatus.set@odatatype('microsoft.graph.security.retentionEventStatus');


requestBody.setEventStatus($eventStatus);
requestBody.setLastStatusUpdateDateTime(DateTime('String (timestamp)'));



result = awaitclient.security().triggers().retentionEvents().post(requestBody);


```