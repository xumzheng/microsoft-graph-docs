---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CrossTenantAccessPolicy
{
	AllowedCloudEndpoints = new List<string>
	{
		"microsoftonline.us",
		"partner.microsoftonline.cn",
	},
};
await graphClient.Policies.CrossTenantAccessPolicy.PatchAsync(requestBody);


```