---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Me.Events.Item.Accept.AcceptPostRequestBody
{
	Comment = "comment-value",
	SendResponse = true,
};
await graphClient.Me.Events["event-id"].Accept.PostAsync(requestBody);


```