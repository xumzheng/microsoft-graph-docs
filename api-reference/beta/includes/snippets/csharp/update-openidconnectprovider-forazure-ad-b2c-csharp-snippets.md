---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProviderBase
{
	OdataType = "#microsoft.graph.socialIdentityProvider",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"responseType" , "id_token"
		},
	},
};
await graphClient.Identity.IdentityProviders["identityProviderBase-id"].PatchAsync(requestBody);


```