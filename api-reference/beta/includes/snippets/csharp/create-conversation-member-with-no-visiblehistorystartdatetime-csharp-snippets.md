---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConversationMember
{
	@odata.type = "#microsoft.graph.aadUserConversationMember",
	Roles = new List<String>
	{
		"owner",
	}
	AdditionalData = new()
	{
		{"user@odata.bind", "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"},
	}
};
var result = await graphClient.Chats["chat-id"].Members.PostAsync(requestBody);


```