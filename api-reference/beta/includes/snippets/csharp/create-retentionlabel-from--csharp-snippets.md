---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RetentionLabel
{
	OdataType = "#microsoft.graph.security.retentionLabel",
	DisplayName = "String",
	BehaviorDuringRetentionPeriod = BehaviorDuringRetentionPeriod.String,
	ActionAfterRetentionPeriod = ActionAfterRetentionPeriod.String,
	RetentionTrigger = RetentionTrigger.String,
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
	DefaultRecordBehavior = DefaultRecordBehavior.String,
};
var result = await graphClient.Security.Labels.RetentionLabels.PostAsync(requestBody);


```