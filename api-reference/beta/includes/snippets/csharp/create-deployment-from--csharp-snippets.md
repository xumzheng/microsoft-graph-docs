---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.WindowsUpdates.Deployment
{
	OdataType = "#microsoft.graph.windowsUpdates.deployment",
	Content = new DeployableContent
	{
		OdataType = "microsoft.graph.windowsUpdates.featureUpdateReference",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"version" , "20H2"
			},
		},
	},
	Settings = new DeploymentSettings
	{
		OdataType = "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		Rollout = new RolloutSettings
		{
			DevicesPerOffer = 100,
		},
		Monitoring = new MonitoringSettings
		{
			MonitoringRules = new List<Microsoft.Graph.Beta.Models.WindowsUpdates.MonitoringRule>
			{
				new MonitoringRule
				{
					OdataType = "#microsoft.graph.windowsUpdates.monitoringRule",
					Signal = Microsoft.Graph.Beta.Models.WindowsUpdates.MonitoringSignal.Rollback,
					Threshold = 5,
					Action = Microsoft.Graph.Beta.Models.WindowsUpdates.MonitoringAction.PauseDeployment,
				},
			},
		},
	},
};
var result = await graphClient.Admin.Windows.Updates.Deployments.PostAsync(requestBody);


```