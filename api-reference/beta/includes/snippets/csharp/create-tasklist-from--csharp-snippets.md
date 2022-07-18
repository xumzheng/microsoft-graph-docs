---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BaseTaskList
{
	@odata.type = "#microsoft.graph.taskList",
	DisplayName = "Shopping list",
};
var result = await graphClient.Me.Tasks.Lists.PostAsync(requestBody);


```