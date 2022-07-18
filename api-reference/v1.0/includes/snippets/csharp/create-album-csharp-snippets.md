---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BundlesRequestBody
{
	AdditionalData = new()
	{
		{"name", "My Day at the Beach"},
		{"@microsoft.graph.conflictBehavior", "rename"},
		{"children", new List<Object>
		{
		}
	}
};
await graphClient.Drive.Bundles.PostAsync(requestBody);


```