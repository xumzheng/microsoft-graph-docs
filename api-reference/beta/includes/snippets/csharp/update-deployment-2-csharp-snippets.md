---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Deployment
{
	@odata.type = "#microsoft.graph.windowsUpdates.deployment",
	Settings = new DeploymentSettings
	{
		@odata.type = "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		Monitoring = new MonitoringSettings
		{
			MonitoringRules = new List<MonitoringRule>
			{
				new MonitoringRule
				{
					Signal = "rollback",
					Threshold = 5,
					Action = "pauseDeployment",
				},
			}
		},
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].PatchAsync(requestBody);


```