---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["accessPackageCatalog-id"].AccessPackageResourceRoles.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')";
	requestConfiguration.QueryParameters.Expand = new string []{ "accessPackageResource" };
});


```