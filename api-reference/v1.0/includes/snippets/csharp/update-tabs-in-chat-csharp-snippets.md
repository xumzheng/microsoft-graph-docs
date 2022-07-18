---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TeamsTab
{
	DisplayName = "My Contoso Tab - updated again",
};
await graphClient.Chats["chat-id"].Tabs["teamsTab-id"].PatchAsync(requestBody);


```