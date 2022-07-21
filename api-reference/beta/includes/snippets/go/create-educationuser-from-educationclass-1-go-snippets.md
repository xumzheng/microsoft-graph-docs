---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/beta/education/users/13015"
requestBody.SetOdataId(&odataId) 

graphClient.Education().ClassesById("educationClass-id").Members().$ref().Post(requestBody)


```