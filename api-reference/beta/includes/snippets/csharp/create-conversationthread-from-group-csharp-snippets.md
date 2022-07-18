---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConversationThread
{
	Topic = "New Conversation Thread Topic",
	Posts = new List<Post>
	{
		new Post
		{
			Body = new ItemBody
			{
				ContentType = "html",
				Content = "this is body content",
			},
			NewParticipants = new List<Recipient>
			{
				new Recipient
				{
					AdditionalData = new()
					{
					}
				},
			}
		},
	}
};
var result = await graphClient.Groups["group-id"].Threads.PostAsync(requestBody);


```