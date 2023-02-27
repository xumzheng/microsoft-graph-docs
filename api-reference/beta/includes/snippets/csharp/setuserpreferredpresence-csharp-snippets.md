---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Users.Item.Presence.MicrosoftGraphSetUserPreferredPresence.SetUserPreferredPresencePostRequestBody
{
	Availability = "DoNotDisturb",
	Activity = "DoNotDisturb",
	ExpirationDuration = TimeSpan.Parse("PT8H"),
};
await graphClient.Users["user-id"].Presence.MicrosoftGraphSetUserPreferredPresence.PostAsync(requestBody);


```