---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewEducationOutcome()
odataType := "#microsoft.graph.educationPointsOutcome"
requestBody.SetOdataType(&odataType) 
additionalData := map[string]interface{}{
points := graphmodels.New()
odataType := "#microsoft.graph.educationAssignmentPointsGrade"
points.SetOdataType(&odataType) 
points := int32(85.0)
points.SetPoints(&points) 
	requestBody.SetPoints(points)
}
requestBody.SetAdditionalData(additionalData)

graphClient.Education().ClassesById("educationClass-id").AssignmentsById("educationAssignment-id").SubmissionsById("educationSubmission-id").OutcomesById("educationOutcome-id").Patch(requestBody)


```