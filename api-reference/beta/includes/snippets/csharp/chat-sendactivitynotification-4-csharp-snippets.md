---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SendActivityNotificationRequestBody
{
	Topic = new TeamworkActivityTopic
	{
		Source = "entityUrl",
		Value = "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2",
	},
	ActivityType = "taskCreated",
	PreviewText = new ItemBody
	{
		Content = "New Task Created",
	},
	Recipient = new TeamworkNotificationRecipient
	{
		@odata.type = "microsoft.graph.chatMembersNotificationRecipient",
		AdditionalData = new()
		{
			{"chatId", "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"},
		}
	},
	TemplateParameters = new List<KeyValuePair>
	{
		new KeyValuePair
		{
			Name = "taskId",
			Value = "Task 12322",
		},
	}
};
await graphClient.Chats["chat-id"].SendActivityNotification.PostAsync(requestBody);


```