---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.DirectoryNamespace.AdministrativeUnits.Item.Members.MembersPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.type" , "#Microsoft.Graph.Group"
		},
		{
			"description" , "Self help community for golf"
		},
		{
			"displayName" , "Golf Assist"
		},
		{
			"groupTypes" , new List<string>
			{
				"Unified",
			}
		},
		{
			"mailEnabled" , true
		},
		{
			"mailNickname" , "golfassist"
		},
		{
			"securityEnabled" , false
		},
	},
};
await graphClient.DirectoryObject.AdministrativeUnits["administrativeUnit-id"].Members.PostAsync(requestBody);


```