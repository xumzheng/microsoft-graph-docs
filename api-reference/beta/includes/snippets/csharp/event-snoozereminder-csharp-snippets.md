---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Me.Events.Item.SnoozeReminder.SnoozeReminderPostRequestBody
{
	NewReminderTime = new DateTimeTimeZone
	{
		DateTime = "2016-10-19T10:37:00Z",
		TimeZone = "timeZone-value",
	},
};
await graphClient.Me.Events["event-id"].SnoozeReminder.PostAsync(requestBody);


```