---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Chats.Item.UnhideForUser.UnhideForUserPostRequestBody
{
	User = new TeamworkUserIdentity
	{
		Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"tenantId" , "2a690434-97d9-4eed-83a6-f5f13600199a"
			},
		},
	},
};
await graphClient.Chats["chat-id"].UnhideForUser.PostAsync(requestBody);


```