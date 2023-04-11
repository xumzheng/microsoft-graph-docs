---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RetentionEvent()
request_body.@odatatype = '#microsoft.graph.security.retentionEvent'

request_body.displayName = 'String'

request_body.description = 'String'

eventQueriesEventQuery1 = EventQuery()
eventQueriesEventQuery1.@odatatype = 'microsoft.graph.security.eventQueries'


eventQueriesArray []= eventQueriesEventQuery1;
request_body.eventqueries(eventQueriesArray)


request_body.eventTriggerDateTime = DateTime('String (timestamp)')

createdBy = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.createdBy = createdBy
eventPropagationResultsEventPropagationResult1 = EventPropagationResult()
eventPropagationResultsEventPropagationResult1.@odatatype = 'microsoft.graph.security.eventPropagationResult'


eventPropagationResultsArray []= eventPropagationResultsEventPropagationResult1;
request_body.eventpropagationresults(eventPropagationResultsArray)


eventStatus = RetentionEventStatus()
eventStatus.@odatatype = 'microsoft.graph.security.retentionEventStatus'


request_body.eventStatus = eventStatus
request_body.lastStatusUpdateDateTime = DateTime('String (timestamp)')



request_configuration = RetentionEventsRequestBuilderPostRequestConfiguration(
)


result = await client.security.triggers.retentionEvents.post(request_body = request_body)


```