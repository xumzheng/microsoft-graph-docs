---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Drive.Bundles.BundlesPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"name" , "My Day at the Beach"
		},
		{
			"@microsoft.graph.conflictBehavior" , "rename"
		},
		{
			"bundle" , new 
			{
				Album = new 
				{
				},
			}
		},
		{
			"children" , new List<>
			{
				new 
				{
					Id = "1234asdf",
				},
			}
		},
	},
};
await graphClient.Drive.Bundles.PostAsync(requestBody);


```