---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Chats.Item.SendActivityNotification.SendActivityNotificationPostRequestBody
{
	Topic = new TeamworkActivityTopic
	{
		Source = TeamworkActivityTopicSource.Text,
		Value = "Weekly Virtual Social",
		WebUrl = "Teams webUrl",
	},
	PreviewText = new ItemBody
	{
		Content = "It will be fun!",
	},
	ActivityType = "eventCreated",
	Recipient = new TeamworkNotificationRecipient
	{
		OdataType = "microsoft.graph.chatMembersNotificationRecipient",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"chatId" , "19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"
			},
		},
	},
};
await graphClient.Chats["chat-id"].SendActivityNotification.PostAsync(requestBody);


```