---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EnrollAssetsPostRequestBody
{
	UpdateCategory = UpdateCategory.String,
	Assets = new List<UpdatableAsset>
	{
		new UpdatableAsset
		{
			OdataType = "#microsoft.graph.windowsUpdates.azureADDevice",
			Id = "String (identifier)",
		},
	},
};
await graphClient.Admin.Windows.Updates.UpdatableAssets.EnrollAssets.PostAsync(requestBody);


```