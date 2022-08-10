---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BundlesPostRequestBody
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"name" , "Just some files"
		},
		{
			"@microsoft.graph.conflictBehavior" , "rename"
		},
		{
			"bundle" , new 
			{
			}
		},
		{
			"children" , new List<>
			{
				new 
				{
					Id = "1234asdf",
				},
				new 
				{
					Id = "1234qwerty",
				},
			}
		},
	},
};
await graphClient.Drive.Bundles.PostAsync(requestBody);


```