---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OnlineMeeting
{
	LobbyBypassSettings = new LobbyBypassSettings
	{
		IsDialInBypassEnabled = true,
	},
};
var result = await graphClient.Me.OnlineMeetings["onlineMeeting-id"].PatchAsync(requestBody);


```