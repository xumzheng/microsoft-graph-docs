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
			ContentType = "text",
			Content = "I attached an event.",
		},
		Attachments = new List<Attachment>
		{
			new Attachment
			{
				@odata.type = "#microsoft.graph.itemAttachment",
				Name = "Holiday event",
				AdditionalData = new()
				{
				}
			},
		}
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Reply.PostAsync(requestBody);


```