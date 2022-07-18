---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChatMessage
{
	MessageType = "message",
	Subject = null,
	Summary = null,
	Importance = "normal",
	Locale = "en-us",
	From = new 
	{
		Application = null,
		Device = null,
		User = new Identity
		{
			Id = "3b102402-813e-4e17-a6b2-f841aef1fdfc",
			DisplayName = "Sumit Gupta",
			AdditionalData = new()
			{
				{"userIdentityType", "aadUser"},
			}
		},
		AdditionalData = new()
		{
			{"conversation", null},
		}
	},
	Body = new ItemBody
	{
		ContentType = "text",
		Content = "Edit text only",
	},
	Attachments = new List<ChatMessageAttachment>
	{
	}
	Mentions = new List<ChatMessageMention>
	{
	}
	Reactions = new List<ChatMessageReaction>
	{
	}
};
await graphClient.Teams["team-id"].Channels["channel-id"].Messages["chatMessage-id"].PatchAsync(requestBody);


```