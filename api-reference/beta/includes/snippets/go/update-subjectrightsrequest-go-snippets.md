---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewSubjectRightsRequest()
odataType := "#microsoft.graph.subjectRightsRequest"
requestBody.SetOdataType(&odataType) 
internalDueDateTime , err := time.Parse(time.RFC3339, "2021-08-30T00:00:00Z")
requestBody.SetInternalDueDateTime(&internalDueDateTime) 

graphClient.Privacy().SubjectRightsRequestsById("subjectRightsRequest-id").Patch(requestBody)


```