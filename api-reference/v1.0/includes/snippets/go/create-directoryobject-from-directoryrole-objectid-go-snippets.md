---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca"
requestBody.SetOdataId(&odataId) 

graphClient.DirectoryRolesById("directoryRole-id").Members().$ref().Post(requestBody)


```