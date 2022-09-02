---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.RetentionLabel
{
	OdataType = "#microsoft.graph.security.retentionLabel",
	DisplayName = "String",
	BehaviorDuringRetentionPeriod = Microsoft.Graph.Beta.Models.Security.BehaviorDuringRetentionPeriod.String,
	ActionAfterRetentionPeriod = Microsoft.Graph.Beta.Models.Security.ActionAfterRetentionPeriod.String,
	RetentionTrigger = Microsoft.Graph.Beta.Models.Security.RetentionTrigger.String,
	RetentionDuration = new RetentionDuration
	{
		OdataType = "microsoft.graph.security.retentionDuration",
	},
	IsInUse = boolean,
	DescriptionForAdmins = "String",
	DescriptionForUsers = "String",
	CreatedBy = new IdentitySet
	{
		OdataType = "microsoft.graph.identitySet",
	},
	LabelToBeApplied = "String",
	DefaultRecordBehavior = Microsoft.Graph.Beta.Models.Security.DefaultRecordBehavior.String,
};
await graphClient.Security.Labels.RetentionLabels["retentionLabel-id"].PatchAsync(requestBody);


```