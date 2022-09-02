---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PermissionGrantPolicy
{
	DisplayName = "Custom permission grant policy",
};
await graphClient.Policies.PermissionGrantPolicies["permissionGrantPolicy-id"].PatchAsync(requestBody);


```