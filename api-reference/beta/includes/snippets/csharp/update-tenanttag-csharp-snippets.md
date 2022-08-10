---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TenantTag
{
	DisplayName = "Onboarding",
	Description = "Tenants that we are currently onboarding",
};
await graphClient.TenantRelationships.ManagedTenants.TenantTags["tenantTag-id"].PatchAsync(requestBody);


```