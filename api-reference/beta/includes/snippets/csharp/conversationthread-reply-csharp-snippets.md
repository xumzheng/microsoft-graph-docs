---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PostRequestBody
{
	Post = new Post
	{
		Body = new ItemBody
		{
			ContentType = "",
			Content = "content-value",
		},
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Reply.PostAsync(requestBody);


```