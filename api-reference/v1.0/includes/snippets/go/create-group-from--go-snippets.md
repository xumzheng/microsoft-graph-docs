---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/v1.0/groups/{groupId}"
requestBody.SetOdataId(&odataId) 

graphClient.Print().SharesById("printerShare-id").AllowedGroups().$ref().Post(requestBody)


```