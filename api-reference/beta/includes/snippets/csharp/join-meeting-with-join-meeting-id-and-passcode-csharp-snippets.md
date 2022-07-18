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
	MeetingInfo = new MeetingInfo
	{
		@odata.type = "#microsoft.graph.joinMeetingIdMeetingInfo",
		AdditionalData = new()
		{
			{"joinMeetingId", "1234567"},
			{"passcode", "psw123"},
		}
	},
	TenantId = "86dc81db-c112-4228-9222-63f3esaa1edb",
};
var result = await graphClient.Communications.Calls.PostAsync(requestBody);


```