---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AppManagementPolicie
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.id" , "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"
		},
	},
};
await graphClient.ServicePrincipals["servicePrincipal-id"].AppManagementPolicies["appManagementPolicy-id"].PostAsync(requestBody);


```