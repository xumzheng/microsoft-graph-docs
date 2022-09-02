---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SendActivityNotificationPostRequestBody
{
	Topic = new TeamworkActivityTopic
	{
		Source = TeamworkActivityTopicSource.Entityurl,
		Value = "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}",
	},
	ActivityType = "taskCreated",
	PreviewText = new ItemBody
	{
		Content = "New Task Created",
	},
	TemplateParameters = new List<KeyValuePair>
	{
		new KeyValuePair
		{
			Name = "taskId",
			Value = "Task 12322",
		},
	},
};
await graphClient.Users["user-id"].Teamwork.SendActivityNotification.PostAsync(requestBody);


```