---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SetPresencePostRequestBody
{
	SessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87",
	Availability = "Available",
	Activity = "Available",
	ExpirationDuration = TimeSpan.Parse("PT1H"),
};
await graphClient.Users["user-id"].Presence.SetPresence.PostAsync(requestBody);


```