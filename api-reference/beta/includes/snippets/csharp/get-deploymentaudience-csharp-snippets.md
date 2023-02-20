---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deploymentAudience = await graphClient.Admin.Windows.Updates.DeploymentAudiences["{windowsUpdates.deploymentAudience-id}"]
	.Request()
	.GetAsync();

```