---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConditionalAccessPolicy
{
	DisplayName = "Block access to EXO non-trusted regions.",
	State = ConditionalAccessPolicyState.Enabled,
	Conditions = new ConditionalAccessConditionSet
	{
		ClientAppTypes = new List<>
		{
			"all",
		},
		Applications = new ConditionalAccessApplications
		{
			IncludeApplications = new List<>
			{
				"00000002-0000-0ff1-ce00-000000000000",
			},
		},
		Users = new ConditionalAccessUsers
		{
			IncludeGroups = new List<>
			{
				"ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba",
			},
		},
		Locations = new ConditionalAccessLocations
		{
			IncludeLocations = new List<>
			{
				"198ad66e-87b3-4157-85a3-8a7b51794ee9",
			},
		},
	},
	GrantControls = new ConditionalAccessGrantControls
	{
		Operator = "OR",
		BuiltInControls = new List<>
		{
			"block",
		},
	},
};
var result = await graphClient.Identity.ConditionalAccess.Policies.PostAsync(requestBody);


```