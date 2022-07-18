---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChatMessage
{
	Body = new ItemBody
	{
		ContentType = "html",
		Content = "<div><div><at id="0">GraphTesting</at>&nbsp;Hello team</div></div>",
	},
	Mentions = new List<ChatMessageMention>
	{
		new ChatMessageMention
		{
			Id = 0,
			MentionText = "GraphTesting",
			Mentioned = new 
			{
				Conversation = new 
				{
					Id = "68a3e365-f7d9-4a56-b499-24332a9cc572",
					DisplayName = "GraphTesting",
					ConversationIdentityType = "team",
				},
			},
		},
	}
	Reactions = new List<ChatMessageReaction>
	{
	}
};
var result = await graphClient.Teams["team-id"].Channels["channel-id"].Messages.PostAsync(requestBody);


```