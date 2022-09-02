---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Extension
{
	OdataType = "#microsoft.outlookServices.openTypeExtension",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"extensionName" , "Com.Contoso.Estimate"
		},
		{
			"companyName" , "Contoso"
		},
		{
			"expirationDate" , "2016-07-30T11:00:00.000Z"
		},
		{
			"DealValue" , 1010100
		},
		{
			"topPicks" , new List<>
			{
				"Employees only",
				"Add spouse or guest",
				"Add family",
			}
		},
	},
};
await graphClient.Groups["group-id"].Threads["conversationThread-id"].Posts["post-id"].Extensions["extension-id"].PatchAsync(requestBody);


```