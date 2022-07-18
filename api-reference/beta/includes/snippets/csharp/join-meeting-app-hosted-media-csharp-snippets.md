---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Call
{
	@odata.type = "#microsoft.graph.call",
	Direction = "outgoing",
	CallbackUri = "https://bot.contoso.com/callback",
	RequestedModalities = new List<Modality>
	{
		"audio",
	}
	MediaConfig = new MediaConfig
	{
		@odata.type = "#microsoft.graph.appHostedMediaConfig",
		AdditionalData = new()
		{
			{"blob", "<Media Session Configuration>"},
		}
	},
	ChatInfo = new ChatInfo
	{
		ThreadId = "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
		MessageId = "0",
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
	TenantId = "aa67bd4c-8475-432d-bd41-39f255720e0a",
};
var result = await graphClient.Communications.Calls.PostAsync(requestBody);


```