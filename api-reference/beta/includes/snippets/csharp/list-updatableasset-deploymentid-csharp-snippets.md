---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Admin.Windows.Updates.DeploymentAudiences["{windowsUpdates.deploymentAudience-id}"].Members
	.Request()
	.GetAsync();

```