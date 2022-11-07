---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new LinkedResource
{
	OdataType = "#microsoft.graph.linkedResource",
	WebUrl = "http://microsoft.com",
	ApplicationName = "Microsoft",
	DisplayName = "Microsoft",
};
var result = await graphClient.Me.Todo.Lists["todoTaskList-id"].Tasks["todoTask-id"].LinkedResources["linkedResource-id"].PatchAsync(requestBody);


```