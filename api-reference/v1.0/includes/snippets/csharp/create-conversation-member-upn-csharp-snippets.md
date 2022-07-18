---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConversationMember
{
	@odata.type = "#microsoft.graph.aadUserConversationMember",
	VisibleHistoryStartDateTime = DateTimeOffset.Parse("2019-04-18T23:51:43.255Z"),
	Roles = new List<String>
	{
		"owner",
	}
	AdditionalData = new()
	{
		{"user@odata.bind", "https://graph.microsoft.com/v1.0/users/jacob@contoso.com"},
	}
};
var result = await graphClient.Chats["chat-id"].Members.PostAsync(requestBody);


```