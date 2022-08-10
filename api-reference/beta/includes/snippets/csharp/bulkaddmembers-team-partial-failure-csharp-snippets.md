---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AddPostRequestBody
{
	Values = new List<ConversationMember>
	{
		new ConversationMember
		{
			OdataType = "microsoft.graph.aadUserConversationMember",
			Roles = new List<>
			{
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"user@odata.bind" , "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
				},
			},
		},
		new ConversationMember
		{
			OdataType = "microsoft.graph.aadUserConversationMember",
			Roles = new List<>
			{
				"owner",
			},
			AdditionalData = new Dictionary<string, object>
			{
				{
					"user@odata.bind" , "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
				},
			},
		},
	},
};
var result = await graphClient.Teams["team-id"].Members.Add.PostAsync(requestBody);


```