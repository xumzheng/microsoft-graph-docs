---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SendActivityNotificationToRecipientsRequestBody
{
	Topic = new TeamworkActivityTopic
	{
		Source = "entityUrl",
		Value = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}",
	},
	ActivityType = "pendingFinanceApprovalRequests",
	PreviewText = new ItemBody
	{
		Content = "Internal spending team has a pending finance approval requests",
	},
	Recipients = new List<TeamworkNotificationRecipient>
	{
		new TeamworkNotificationRecipient
		{
			@odata.type = "microsoft.graph.aadUserNotificationRecipient",
			AdditionalData = new()
			{
				{"userId", "569363e2-4e49-4661-87f2-16f245c5d66a"},
			}
		},
		new TeamworkNotificationRecipient
		{
			@odata.type = "microsoft.graph.aadUserNotificationRecipient",
			AdditionalData = new()
			{
				{"userId", "ab88234e-0874-477c-9638-d144296ed04f"},
			}
		},
		new TeamworkNotificationRecipient
		{
			@odata.type = "microsoft.graph.aadUserNotificationRecipient",
			AdditionalData = new()
			{
				{"userId", "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"},
			}
		},
	}
	TemplateParameters = new List<KeyValuePair>
	{
		new KeyValuePair
		{
			Name = "pendingRequestCount",
			Value = "5",
		},
	}
};
await graphClient.Teamwork.SendActivityNotificationToRecipients.PostAsync(requestBody);


```