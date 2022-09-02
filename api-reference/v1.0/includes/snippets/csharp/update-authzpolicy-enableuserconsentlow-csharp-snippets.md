---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthorizationPolicy
{
	DefaultUserRolePermissions = new DefaultUserRolePermissions
	{
		PermissionGrantPoliciesAssigned = new List<>
		{
			"managePermissionGrantsForSelf.microsoft-user-default-low",
		},
	},
};
await graphClient.Policies.AuthorizationPolicy.PatchAsync(requestBody);


```