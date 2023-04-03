---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.WindowsUpdates.ComplianceChange
{
	OdataType = "#microsoft.graph.windowsUpdates.contentApproval",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"content" , new Content
			{
				OdataType = "#microsoft.graph.windowsUpdates.catalogContent",
				CatalogEntry = new CatalogEntry
				{
					OdataType = "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
					Id = "6b7e60db-a8e4-426a-9aed-bd12b5c0b9d4",
				},
			}
		},
		{
			"deploymentSettings" , new DeploymentSettings
			{
			}
		},
		{
			"schedule" , new Schedule
			{
				StartDateTime = "String (timestamp)",
				GradualRollout = new GradualRollout
				{
					OdataType = "#microsoft.graph.windowsUpdates.dateDrivenRolloutSettings",
					EndDateTime = "String (timestamp)",
				},
			}
		},
	},
};
var result = await graphClient.Admin.Windows.Updates.UpdatePolicies["{updatePolicy-id}"].ComplianceChanges.PostAsync(requestBody);


```