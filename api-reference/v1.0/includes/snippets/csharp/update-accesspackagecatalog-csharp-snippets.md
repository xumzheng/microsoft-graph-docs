---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageCatalog
{
	DisplayName = "Catalog One",
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.Catalogs["accessPackageCatalog-id"].PatchAsync(requestBody);


```