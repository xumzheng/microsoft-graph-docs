---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Call
{
	@odata.type = "#microsoft.graph.call",
	CallbackUri = "https://bot.contoso.com/callback",
	RequestedModalities = new List<Modality>
	{
		"audio",
	}
	MediaConfig = new MediaConfig
	{
		@odata.type = "#microsoft.graph.serviceHostedMediaConfig",
		AdditionalData = new()
		{
			{"preFetchMedia", new List<Object>
			{
			}
		}
	},
	ChatInfo = new ChatInfo
	{
		ThreadId = "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
		MessageId = "1533758867081",
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.chatInfo"},
		}
	},
	MeetingInfo = new MeetingInfo
	{
		@odata.type = "#microsoft.graph.organizerMeetingInfo",
		AllowConversationWithoutHost = true,
		AdditionalData = new()
		{
		}
	},
};
var result = await graphClient.Communications.Calls.PostAsync(requestBody);


```