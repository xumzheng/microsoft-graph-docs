---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/v1.0/education/classes/11006"
requestBody.SetOdataId(&odataId) 

graphClient.Education().SchoolsById("educationSchool-id").Classes().$ref().Post(requestBody)


```