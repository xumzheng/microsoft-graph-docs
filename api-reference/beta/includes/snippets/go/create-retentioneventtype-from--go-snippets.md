---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewRetentionEventType()
odataType := "#microsoft.graph.security.retentionEventType"
requestBody.SetOdataType(&odataType) 
displayName := "String"
requestBody.SetDisplayName(&displayName) 
description := "String"
requestBody.SetDescription(&description) 
createdBy := graphmodels.NewIdentitySet()
odataType := "microsoft.graph.identitySet"
createdBy.SetOdataType(&odataType) 
requestBody.SetCreatedBy(createdBy)

result, err := graphClient.Security().TriggerTypes().RetentionEventTypes().Post(requestBody)


```