---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ServicePrincipalIdsRequestBody
{
	ServicePrincipalIds = new List<String>
	{
		"9089a539-a539-9089-39a5-899039a58990",
	}
};
await graphClient.IdentityProtection.RiskyServicePrincipals.Dismiss.PostAsync(requestBody);


```