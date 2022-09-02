---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Admin.Windows.Updates.Deployments.Item.Audience.UpdateAudience.UpdateAudiencePostRequestBody
{
	AddMembers = new List<Microsoft.Graph.Beta.Models.WindowsUpdates.UpdatableAsset>
	{
		new UpdatableAsset
		{
			OdataType = "#microsoft.graph.windowsUpdates.azureADDevice",
			Id = "String (identifier)",
		},
	},
	RemoveMembers = new List<Microsoft.Graph.Beta.Models.WindowsUpdates.UpdatableAsset>
	{
		new UpdatableAsset
		{
			OdataType = "#microsoft.graph.windowsUpdates.azureADDevice",
			Id = "String (identifier)",
		},
	},
	AddExclusions = new List<Microsoft.Graph.Beta.Models.WindowsUpdates.UpdatableAsset>
	{
		new UpdatableAsset
		{
			OdataType = "#microsoft.graph.windowsUpdates.azureADDevice",
			Id = "String (identifier)",
		},
	},
	RemoveExclusions = new List<Microsoft.Graph.Beta.Models.WindowsUpdates.UpdatableAsset>
	{
		new UpdatableAsset
		{
			OdataType = "#microsoft.graph.windowsUpdates.azureADDevice",
			Id = "String (identifier)",
		},
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].Audience.UpdateAudience.PostAsync(requestBody);


```