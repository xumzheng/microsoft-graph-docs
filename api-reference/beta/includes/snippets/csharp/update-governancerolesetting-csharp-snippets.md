---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new GovernanceRoleSetting
{
	AdminEligibleSettings = new List<GovernanceRuleSetting>
	{
		new GovernanceRuleSetting
		{
			RuleIdentifier = "ExpirationRule",
			Setting = "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}",
		},
	},
};
var result = await graphClient.PrivilegedAccess["privilegedAccess-id"].RoleSettings["governanceRoleSetting-id"].PatchAsync(requestBody);


```