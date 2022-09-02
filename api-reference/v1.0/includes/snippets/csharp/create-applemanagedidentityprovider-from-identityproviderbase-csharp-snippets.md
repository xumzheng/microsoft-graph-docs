---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProviderBase
{
	OdataType = "microsoft.graph.appleManagedIdentityProvider",
	DisplayName = "Sign in with Apple",
	AdditionalData = new Dictionary<string, object>
	{
		{
			"developerId" , "UBF8T346G9"
		},
		{
			"serviceId" , "com.microsoft.rts.b2c.test.client"
		},
		{
			"keyId" , "99P6D879C4"
		},
		{
			"certificateData" , "******"
		},
	},
};
var result = await graphClient.Identity.IdentityProviders.PostAsync(requestBody);


```