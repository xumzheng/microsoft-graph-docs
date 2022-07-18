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
		Value = "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}",
	},
	ActivityType = "approvalRequired",
	PreviewText = new ItemBody
	{
		Content = "Deployment requires your approval",
	},
	Recipient = new TeamworkNotificationRecipient
	{
		@odata.type = "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
		AdditionalData = new()
		{
			{"userId", "jacob@contoso.com"},
		}
	},
	TemplateParameters = new List<KeyValuePair>
	{
		new KeyValuePair
		{
			Name = "approvalTaskId",
			Value = "2020AAGGTAPP",
		},
	}
};
await graphClient.Chats["chat-id"].SendActivityNotification.PostAsync(requestBody);


```