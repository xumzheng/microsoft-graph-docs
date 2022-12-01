---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConversationThread
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"originalStartTimeZone" , "originalStartTimeZone-value"
		},
		{
			"originalEndTimeZone" , "originalEndTimeZone-value"
		},
		{
			"responseStatus" , new 
			{
				Response = "",
				Time = "datetime-value",
			}
		},
		{
			"iCalUId" , "iCalUId-value"
		},
		{
			"reminderMinutesBeforeStart" , 99
		},
		{
			"isReminderOn" , true
		},
	},
};
var result = await graphClient.Groups["group-id"].Threads["conversationThread-id"].PatchAsync(requestBody);


```