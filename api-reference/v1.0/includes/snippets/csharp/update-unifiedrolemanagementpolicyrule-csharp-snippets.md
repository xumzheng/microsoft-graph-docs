---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleManagementPolicyRule
{
	OdataType = "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
	Id = "Expiration_EndUser_Assignment",
	Target = new UnifiedRoleManagementPolicyRuleTarget
	{
		OdataType = "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
		Caller = "EndUser",
		Operations = new List<>
		{
			"All",
		},
		Level = "Assignment",
		InheritableSettings = new List<>
		{
		},
		EnforcedSettings = new List<>
		{
		},
	},
	AdditionalData = new Dictionary<string, object>
	{
		{
			"isExpirationRequired" , true
		},
		{
			"maximumDuration" , "PT1H45M"
		},
	},
};
await graphClient.Policies.RoleManagementPolicies["unifiedRoleManagementPolicy-id"].Rules["unifiedRoleManagementPolicyRule-id"].PatchAsync(requestBody);


```