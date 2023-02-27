---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CrossTenantAccessPolicy
{
	DisplayName = "CrossTenantAccessPolicy",
};
var result = await graphClient.Policies.CrossTenantAccessPolicy.PatchAsync(requestBody);


```