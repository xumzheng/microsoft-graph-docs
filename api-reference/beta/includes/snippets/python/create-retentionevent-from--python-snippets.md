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

event_queries_event_query1 = EventQuery()
eventQueriesEventQuery1.@odatatype = 'microsoft.graph.security.eventQueries'


eventQueriesArray []= eventQueriesEventQuery1;
request_body.eventqueries(eventQueriesArray)


request_body.eventTriggerDateTime = DateTime('String (timestamp)')

created_by = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.created_by = createdBy
event_propagation_results_event_propagation_result1 = EventPropagationResult()
eventPropagationResultsEventPropagationResult1.@odatatype = 'microsoft.graph.security.eventPropagationResult'


eventPropagationResultsArray []= eventPropagationResultsEventPropagationResult1;
request_body.eventpropagationresults(eventPropagationResultsArray)


event_status = RetentionEventStatus()
eventStatus.@odatatype = 'microsoft.graph.security.retentionEventStatus'


request_body.event_status = eventStatus
request_body.lastStatusUpdateDateTime = DateTime('String (timestamp)')




result = await client.security.triggers.retentionEvents.post(request_body = request_body)


```