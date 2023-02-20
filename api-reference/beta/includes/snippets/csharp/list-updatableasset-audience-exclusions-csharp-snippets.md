---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var exclusions = await graphClient.Admin.Windows.Updates.DeploymentAudiences["{windowsUpdates.deploymentAudience-id}"].Exclusions
	.Request()
	.GetAsync();

```