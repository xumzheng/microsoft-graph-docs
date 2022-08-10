---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new TenantCustomizedInformation
{
	OdataType = "#microsoft.graph.managedTenants.tenantCustomizedInformation",
	TenantId = "String",
	Contacts = new List<TenantContactInformation>
	{
		new TenantContactInformation
		{
			OdataType = "microsoft.graph.managedTenants.tenantContactInformation",
			Name = "String",
			Title = "String",
			Email = "String",
			Phone = "String",
			Notes = "String",
		},
	},
	Website = "String",
};
await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation["tenantCustomizedInformation-id"].PatchAsync(requestBody);


```