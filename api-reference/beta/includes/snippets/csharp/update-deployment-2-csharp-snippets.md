---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..WindowsUpdates.Deployment
{
	OdataType = "#microsoft.graph.windowsUpdates.deployment",
	Settings = new DeploymentSettings
	{
		OdataType = "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		Monitoring = new MonitoringSettings
		{
			MonitoringRules = new List<Microsoft.Graph.Beta..WindowsUpdates.MonitoringRule>
			{
				new MonitoringRule
				{
					Signal = MonitoringSignal.Rollback,
					Threshold = 5,
					Action = MonitoringAction.Pausedeployment,
				},
			},
		},
	},
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].PatchAsync(requestBody);


```