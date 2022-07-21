---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewRetentionEvent()
odataType := "#microsoft.graph.security.retentionEvent"
requestBody.SetOdataType(&odataType) 
displayName := "String"
requestBody.SetDisplayName(&displayName) 
description := "String"
requestBody.SetDescription(&description) 


eventQuery := graphmodels.NewEventQuery()
odataType := "microsoft.graph.security.eventQueries"
eventQuery.SetOdataType(&odataType) 

eventQueries := []graphmodels.EventQueryable {
	eventQuery,

}
requestBody.SetEventQueries(eventQueries)
eventTriggerDateTime , err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetEventTriggerDateTime(&eventTriggerDateTime) 
createdBy := graphmodels.NewIdentitySet()
odataType := "microsoft.graph.identitySet"
createdBy.SetOdataType(&odataType) 
requestBody.SetCreatedBy(createdBy)


eventPropagationResult := graphmodels.NewEventPropagationResult()
odataType := "microsoft.graph.security.eventPropagationResult"
eventPropagationResult.SetOdataType(&odataType) 

eventPropagationResults := []graphmodels.EventPropagationResultable {
	eventPropagationResult,

}
requestBody.SetEventPropagationResults(eventPropagationResults)
eventStatus := graphmodels.NewRetentionEventStatus()
odataType := "microsoft.graph.security.retentionEventStatus"
eventStatus.SetOdataType(&odataType) 
requestBody.SetEventStatus(eventStatus)
lastStatusUpdateDateTime , err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetLastStatusUpdateDateTime(&lastStatusUpdateDateTime) 

result, err := graphClient.Security().Triggers().RetentionEvents().Post(requestBody)


```