---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Deployment
{
	@odata.type = "#microsoft.graph.windowsUpdates.deployment",
	Content = new DeployableContent
	{
		@odata.type = "microsoft.graph.windowsUpdates.featureUpdateReference",
		AdditionalData = new()
		{
			{"version", "20H2"},
		}
	},
	Settings = new DeploymentSettings
	{
		@odata.type = "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		Rollout = new RolloutSettings
		{
			DevicesPerOffer = 100,
		},
		Monitoring = new MonitoringSettings
		{
			MonitoringRules = new List<MonitoringRule>
			{
				new MonitoringRule
				{
					Signal = "rollback",
					Threshold = 5,
					Action = "pauseDeployment",
					AdditionalData = new()
					{
						{"@odata.type", "#microsoft.graph.windowsUpdates.monitoringRule"},
					}
				},
			}
		},
	},
};
var result = await graphClient.Admin.Windows.Updates.Deployments.PostAsync(requestBody);


```