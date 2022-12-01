---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Shares.Item.Permission.Grant.GrantPostRequestBody
{
	Recipients = new List<DriveRecipient>
	{
		new DriveRecipient
		{
			Email = "john@contoso.com",
		},
		new DriveRecipient
		{
			Email = "ryan@external.com",
		},
	},
	Roles = new List<string>
	{
		"read",
	},
};
var result = await graphClient.Shares["sharedDriveItem-id"].Permission.Grant.PostAsync(requestBody);


```