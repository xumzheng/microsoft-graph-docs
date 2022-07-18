---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RetentionLabel
{
	@odata.type = "#microsoft.graph.security.retentionLabel",
	DisplayName = "String",
	BehaviorDuringRetentionPeriod = "String",
	ActionAfterRetentionPeriod = "String",
	RetentionTrigger = "String",
	RetentionDuration = new RetentionDuration
	{
		@odata.type = "microsoft.graph.security.retentionDuration",
	},
	IsInUse = "Boolean",
	DescriptionForAdmins = "String",
	DescriptionForUsers = "String",
	CreatedBy = new IdentitySet
	{
		@odata.type = "microsoft.graph.identitySet",
	},
	LabelToBeApplied = "String",
	DefaultRecordBehavior = "String",
};
var result = await graphClient.Security.Labels.RetentionLabels.PostAsync(requestBody);


```