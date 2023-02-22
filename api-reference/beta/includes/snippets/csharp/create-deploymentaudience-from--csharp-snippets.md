---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deploymentAudience = new Microsoft.Graph.WindowsUpdates.DeploymentAudience
{
};

await graphClient.Admin.Windows.Updates.DeploymentAudiences
	.Request()
	.AddAsync(deploymentAudience);

```