---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Team
{
	DisplayName = "My Sample Team",
	Description = "My Sample Team’s Description",
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
				{"user@odata.bind", "https://graph.microsoft.com/beta/users('jacob@contoso.com')"},
			}
		},
	}
	AdditionalData = new()
	{
		{"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('standard')"},
	}
};
var result = await graphClient.Teams.PostAsync(requestBody);


```