---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
requestBody.SetOdataId(&odataId) 

graphClient.GroupsById("group-id").RejectedSenders().$ref().Post(requestBody)


```