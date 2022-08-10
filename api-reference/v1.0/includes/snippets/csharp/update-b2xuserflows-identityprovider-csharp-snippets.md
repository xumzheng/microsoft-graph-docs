---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProvider
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.id" , "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"
		},
	},
};
await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].IdentityProviders["identityProvider-id"].PostAsync(requestBody);


```