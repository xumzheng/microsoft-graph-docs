---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TodoTaskList
{
	DisplayName = "Vacation Plan",
};
var result = await graphClient.Me.Todo.Lists["todoTaskList-id"].PatchAsync(requestBody);


```