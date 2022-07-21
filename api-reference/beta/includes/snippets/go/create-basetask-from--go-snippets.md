---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewBaseTask()
odataType := "#microsoft.graph.task"
requestBody.SetOdataType(&odataType) 
textBody := "String"
requestBody.SetTextBody(&textBody) 
bodyLastModifiedDateTime , err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetBodyLastModifiedDateTime(&bodyLastModifiedDateTime) 
completedDateTime , err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetCompletedDateTime(&completedDateTime) 
dueDateTime := graphmodels.NewDateTimeTimeZone()
odataType := "microsoft.graph.dateTimeTimeZone"
dueDateTime.SetOdataType(&odataType) 
requestBody.SetDueDateTime(dueDateTime)
startDateTime := graphmodels.NewDateTimeTimeZone()
odataType := "microsoft.graph.dateTimeTimeZone"
startDateTime.SetOdataType(&odataType) 
requestBody.SetStartDateTime(startDateTime)
importance := graphmodels.STRING_IMPORTANCE 
requestBody.SetImportance(&importance) 
recurrence := graphmodels.NewPatternedRecurrence()
odataType := "microsoft.graph.patternedRecurrence"
recurrence.SetOdataType(&odataType) 
requestBody.SetRecurrence(recurrence)
displayName := "String"
requestBody.SetDisplayName(&displayName) 
status := graphmodels.STRING_TASKSTATUS_V2 
requestBody.SetStatus(&status) 
viewpoint := graphmodels.NewTaskViewpoint()
odataType := "microsoft.graph.taskViewpoint"
viewpoint.SetOdataType(&odataType) 
requestBody.SetViewpoint(viewpoint)

result, err := graphClient.Me().Tasks().ListsById("baseTaskList-id").Tasks().Post(requestBody)


```