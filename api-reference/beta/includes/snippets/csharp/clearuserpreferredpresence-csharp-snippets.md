---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Users.Item.Presence.MicrosoftGraphClearUserPreferredPresence.ClearUserPreferredPresencePostRequestBody
{
};
await graphClient.Users["user-id"].Presence.MicrosoftGraphClearUserPreferredPresence.PostAsync(requestBody);


```