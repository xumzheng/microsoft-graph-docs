---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..WindowsUpdates.Deployment
{
	OdataType = "#microsoft.graph.windowsUpdates.deployment",
	State = new DeploymentState
	{
		OdataType = "microsoft.graph.windowsUpdates.deploymentState",
		RequestedValue = RequestedDeploymentStateValue.Paused,
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].PatchAsync(requestBody);


```