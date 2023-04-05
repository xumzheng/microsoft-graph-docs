---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RetentionEvent()
request_body.set@odatatype('#microsoft.graph.security.retentionEvent')

request_body.setDisplayName('String')

request_body.setDescription('String')

eventQueriesEventQuery1 = EventQuery()
eventQueriesEventQuery1.set@odatatype('microsoft.graph.security.eventQueries')


eventQueriesArray []= eventQueriesEventQuery1;
request_body.setEventQueries(eventQueriesArray)


request_body.setEventTriggerDateTime(DateTime('String (timestamp)'))

createdBy = IdentitySet()
createdBy.set@odatatype('microsoft.graph.identitySet')


request_body.setCreatedBy($createdBy)
eventPropagationResultsEventPropagationResult1 = EventPropagationResult()
eventPropagationResultsEventPropagationResult1.set@odatatype('microsoft.graph.security.eventPropagationResult')


eventPropagationResultsArray []= eventPropagationResultsEventPropagationResult1;
request_body.setEventPropagationResults(eventPropagationResultsArray)


eventStatus = RetentionEventStatus()
eventStatus.set@odatatype('microsoft.graph.security.retentionEventStatus')


request_body.setEventStatus($eventStatus)
request_body.setLastStatusUpdateDateTime(DateTime('String (timestamp)'))



result = await client.security_triggers_retentionEvents.post(request_body)


```