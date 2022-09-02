---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChatMessage
{
	MessageType = ChatMessageType.Message,
	Subject = null,
	Summary = null,
	Importance = ChatMessageImportance.Normal,
	Locale = "en-us",
	From = new From
	{
		Application = null,
		Device = null,
		User = new Identity
		{
			Id = "3b102402-813e-4e17-a6b2-f841aef1fdfc",
			DisplayName = "Sumit Gupta",
			AdditionalData = new Dictionary<string, object>
			{
				{
					"userIdentityType" , "aadUser"
				},
			},
		},
		AdditionalData = new Dictionary<string, object>
		{
			{
				"conversation" , null
			},
		},
	},
	Body = new ItemBody
	{
		ContentType = BodyType.Text,
		Content = "Edit text only",
	},
	Attachments = new List<>
	{
	},
	Mentions = new List<>
	{
	},
	Reactions = new List<>
	{
	},
};
await graphClient.Teams["team-id"].Channels["channel-id"].Messages["chatMessage-id"].PatchAsync(requestBody);


```