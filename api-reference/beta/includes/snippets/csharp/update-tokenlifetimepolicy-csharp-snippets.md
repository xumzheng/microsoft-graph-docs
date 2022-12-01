---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TokenLifetimePolicy
{
	Definition = new List<string>
	{
		"definition-value",
	},
	DisplayName = "displayName-value",
	IsOrganizationDefault = true,
};
var result = await graphClient.Policies.TokenLifetimePolicies["tokenLifetimePolicy-id"].PatchAsync(requestBody);


```