---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewEducationOutcome()
odataType := "#microsoft.graph.educationFeedbackResourceOutcome"
requestBody.SetOdataType(&odataType) 
additionalData := map[string]interface{}{
feedbackResource := graphmodels.New()
odataType := "#microsoft.graph.educationWordResource"
feedbackResource.SetOdataType(&odataType) 
displayName := "Document1.docx"
feedbackResource.SetDisplayName(&displayName) 
	requestBody.SetFeedbackResource(feedbackResource)
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Education().ClassesById("educationClass-id").AssignmentsById("educationAssignment-id").SubmissionsById("educationSubmission-id").Outcomes().Post(requestBody)


```