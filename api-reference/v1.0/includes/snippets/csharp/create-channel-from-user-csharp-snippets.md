---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Channel
{
	@odata.type = "#Microsoft.Graph.channel",
	MembershipType = "private",
	DisplayName = "My First Private Channel",
	Description = "This is my first private channels",
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
				{"user@odata.bind", "https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')"},
			}
		},
	}
};
var result = await graphClient.Teams["team-id"].Channels.PostAsync(requestBody);


```