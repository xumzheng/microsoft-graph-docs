---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new $refRequestBody
{
	AdditionalData = new()
	{
		{"@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"},
		{"@odata.type", "#microsoft.graph.identityProvider"},
	}
};
await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].UserFlowIdentityProviders.$ref.PatchAsync(requestBody);


```