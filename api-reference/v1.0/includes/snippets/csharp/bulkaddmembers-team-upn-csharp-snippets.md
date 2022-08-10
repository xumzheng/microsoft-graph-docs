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
					"user@odata.bind" , "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
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
					"user@odata.bind" , "https://graph.microsoft.com/v1.0/users('alex@contoso.com')"
				},
			},
		},
	},
};
var result = await graphClient.Teams["team-id"].Members.Add.PostAsync(requestBody);


```