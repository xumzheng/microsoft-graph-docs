---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BaseTask
{
	OdataType = "#microsoft.graph.task",
	TextBody = "String",
	BodyLastModifiedDateTime = DateTimeOffset.Parse("String (timestamp)"),
	CompletedDateTime = DateTimeOffset.Parse("String (timestamp)"),
	DueDateTime = new DateTimeTimeZone
	{
		OdataType = "microsoft.graph.dateTimeTimeZone",
	},
	StartDateTime = new DateTimeTimeZone
	{
		OdataType = "microsoft.graph.dateTimeTimeZone",
	},
	Importance = Importance.Low,
	Recurrence = new PatternedRecurrence
	{
		OdataType = "microsoft.graph.patternedRecurrence",
	},
	DisplayName = "String",
	Status = TaskStatus_v2.NotStarted,
	Viewpoint = new TaskViewpoint
	{
		OdataType = "microsoft.graph.taskViewpoint",
	},
};
await graphClient.Me.Tasks.Lists["baseTaskList-id"].Tasks["baseTask-id"].PatchAsync(requestBody);


```