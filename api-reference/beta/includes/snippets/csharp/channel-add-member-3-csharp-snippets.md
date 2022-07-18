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
		{"user@odata.bind", "https://graph.microsoft.com/beta/users('jacob@contoso.com')"},
	}
};
var result = await graphClient.Teams["team-id"].Channels["channel-id"].Members.PostAsync(requestBody);


```