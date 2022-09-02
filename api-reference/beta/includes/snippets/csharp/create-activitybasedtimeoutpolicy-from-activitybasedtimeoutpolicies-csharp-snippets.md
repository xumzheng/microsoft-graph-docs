---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ActivityBasedTimeoutPolicy
{
	Definition = new List<>
	{
		"definition-value",
	},
	DisplayName = "displayName-value",
	IsOrganizationDefault = true,
};
var result = await graphClient.Policies.ActivityBasedTimeoutPolicies.PostAsync(requestBody);


```