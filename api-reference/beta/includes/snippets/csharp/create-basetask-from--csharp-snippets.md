---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BaseTask
{
	@odata.type = "#microsoft.graph.task",
	TextBody = "String",
	BodyLastModifiedDateTime = DateTimeOffset.Parse("String (timestamp)"),
	CompletedDateTime = DateTimeOffset.Parse("String (timestamp)"),
	DueDateTime = new DateTimeTimeZone
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.dateTimeTimeZone"},
		}
	},
	StartDateTime = new DateTimeTimeZone
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.dateTimeTimeZone"},
		}
	},
	Importance = "String",
	Recurrence = new PatternedRecurrence
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.patternedRecurrence"},
		}
	},
	DisplayName = "String",
	Status = "String",
	Viewpoint = new TaskViewpoint
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.taskViewpoint"},
		}
	},
};
var result = await graphClient.Me.Tasks.Lists["baseTaskList-id"].Tasks.PostAsync(requestBody);


```