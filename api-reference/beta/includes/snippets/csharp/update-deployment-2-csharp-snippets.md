---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.WindowsUpdates.Deployment
{
	OdataType = "#microsoft.graph.windowsUpdates.deployment",
	Settings = new DeploymentSettings
	{
		OdataType = "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		Monitoring = new MonitoringSettings
		{
			MonitoringRules = new List<Microsoft.Graph.Beta.Models.WindowsUpdates.MonitoringRule>
			{
				new MonitoringRule
				{
					Signal = Microsoft.Graph.Beta.Models.WindowsUpdates.MonitoringSignal.Rollback,
					Threshold = 5,
					Action = Microsoft.Graph.Beta.Models.WindowsUpdates.MonitoringAction.PauseDeployment,
				},
			},
		},
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].PatchAsync(requestBody);


```