---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageCatalog
{
	DisplayName = "sales",
	Description = "for employees working with sales and outside sales partners",
	State = AccessPackageCatalogState.Published,
	IsExternallyVisible = true,
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.Catalogs.PostAsync(requestBody);


```