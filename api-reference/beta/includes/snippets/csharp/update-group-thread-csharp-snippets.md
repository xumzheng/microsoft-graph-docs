---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConversationThread
{
	AdditionalData = new()
	{
		{"originalStartTimeZone", "originalStartTimeZone-value"},
		{"originalEndTimeZone", "originalEndTimeZone-value"},
		{"uid", "iCalUId-value"},
		{"reminderMinutesBeforeStart", },
		{"isReminderOn", true},
	}
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].PatchAsync(requestBody);


```