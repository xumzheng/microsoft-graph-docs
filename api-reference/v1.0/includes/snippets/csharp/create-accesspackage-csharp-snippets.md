---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackage
{
	DisplayName = "sales reps",
	Description = "outside sales representatives",
	IsHidden = false,
	Catalog = new Catalog
	{
		Id = "66584aae-98bb-48cc-9458-7bee5d2a6577",
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages.PostAsync(requestBody);


```