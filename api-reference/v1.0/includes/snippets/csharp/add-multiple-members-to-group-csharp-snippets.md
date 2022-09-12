---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Group
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"members@odata.bind" , new List<string>
			{
				"https://graph.microsoft.com/v1.0/directoryObjects/{id}",
				"https://graph.microsoft.com/v1.0/directoryObjects/{id}",
				"https://graph.microsoft.com/v1.0/directoryObjects/{id}",
			}
		},
	},
};
await graphClient.Groups["group-id"].PatchAsync(requestBody);


```