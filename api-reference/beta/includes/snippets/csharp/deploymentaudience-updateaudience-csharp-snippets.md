---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addMembers = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
	new Microsoft.Graph.WindowsUpdates.AzureADDevice
	{
		Id = "String (identifier)"
	}
};

await graphClient.Admin.Windows.Updates.DeploymentAudiences["{windowsUpdates.deploymentAudience-id}"]
	.UpdateAudience(addMembers,null,null,null)
	.Request()
	.PostAsync();

```