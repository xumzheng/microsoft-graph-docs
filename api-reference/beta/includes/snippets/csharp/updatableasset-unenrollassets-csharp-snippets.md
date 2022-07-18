---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnenrollAssetsRequestBody
{
	UpdateCategory = "String",
	Assets = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.windowsUpdates.azureADDevice"},
				{"id", "String (identifier)"},
			}
		},
	}
};
await graphClient.Admin.Windows.Updates.UpdatableAssets.UnenrollAssets.PostAsync(requestBody);


```