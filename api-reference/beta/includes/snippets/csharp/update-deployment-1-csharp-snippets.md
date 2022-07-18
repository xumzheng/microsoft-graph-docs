---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Deployment
{
	@odata.type = "#microsoft.graph.windowsUpdates.deployment",
	State = new DeploymentState
	{
		RequestedValue = "paused",
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.windowsUpdates.deploymentState"},
		}
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].PatchAsync(requestBody);


```