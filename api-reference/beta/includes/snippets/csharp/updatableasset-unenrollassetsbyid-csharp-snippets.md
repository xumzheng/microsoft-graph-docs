---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnenrollAssetsByIdRequestBody
{
	UpdateCategory = "feature",
	MemberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice",
	Ids = new List<String>
	{
		"String",
		"String",
		"String",
	}
};
await graphClient.Admin.Windows.Updates.UpdatableAssets.UnenrollAssetsById.PostAsync(requestBody);


```