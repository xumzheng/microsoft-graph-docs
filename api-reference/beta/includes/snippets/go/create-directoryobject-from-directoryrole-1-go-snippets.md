---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
requestBody.SetOdataId(&odataId) 

graphClient.DirectoryRolesById("directoryRole-id").Members().$ref().Post(requestBody)


```