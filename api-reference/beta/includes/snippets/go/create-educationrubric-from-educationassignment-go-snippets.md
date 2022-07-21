---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceUpdate()
odataId := "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.Education().ClassesById("educationClass-id").AssignmentsById("educationAssignment-id").Rubric().$ref().Put(requestBody)


```