---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TodoTask
{
	DueDateTime = new DateTimeTimeZone
	{
		DateTime = "2020-07-25T16:00:00",
		TimeZone = "Eastern Standard Time",
	},
};
await graphClient.Me.Todo.Lists["todoTaskList-id"].Tasks["todoTask-id"].PatchAsync(requestBody);


```