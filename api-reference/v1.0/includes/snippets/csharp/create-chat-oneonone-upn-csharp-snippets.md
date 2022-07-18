---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Chat
{
	ChatType = "oneOnOne",
	Members = new List<ConversationMember>
	{
		new ConversationMember
		{
			@odata.type = "#microsoft.graph.aadUserConversationMember",
			Roles = new List<String>
			{
				"owner",
			}
			AdditionalData = new()
			{
				{"user@odata.bind", "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"},
			}
		},
		new ConversationMember
		{
			@odata.type = "#microsoft.graph.aadUserConversationMember",
			Roles = new List<String>
			{
				"owner",
			}
			AdditionalData = new()
			{
				{"user@odata.bind", "https://graph.microsoft.com/v1.0/users('alex@contoso.com')"},
			}
		},
	}
};
var result = await graphClient.Chats.PostAsync(requestBody);


```