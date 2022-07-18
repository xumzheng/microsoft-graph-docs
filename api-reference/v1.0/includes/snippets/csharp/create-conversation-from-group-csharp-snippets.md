---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Conversation
{
	Topic = "Take your wellness days and rest",
	Threads = new List<ConversationThread>
	{
		new ConversationThread
		{
			Posts = new List<Post>
			{
				new Post
				{
					Body = new ItemBody
					{
						ContentType = "html",
						Content = "Contoso cares about you: Rest and Recharge",
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
		},
	}
};
var result = await graphClient.Groups["group-id"].Conversations.PostAsync(requestBody);


```