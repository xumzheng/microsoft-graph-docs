---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TenantCustomizedInformation
{
	@odata.type = "#microsoft.graph.managedTenants.tenantCustomizedInformation",
	TenantId = "String",
	Contacts = new List<TenantContactInformation>
	{
		new TenantContactInformation
		{
			Name = "String",
			Title = "String",
			Email = "String",
			Phone = "String",
			Notes = "String",
			AdditionalData = new()
			{
				{"@odata.type", "microsoft.graph.managedTenants.tenantContactInformation"},
			}
		},
	}
	Website = "String",
};
await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation["tenantCustomizedInformation-id"].PatchAsync(requestBody);


```