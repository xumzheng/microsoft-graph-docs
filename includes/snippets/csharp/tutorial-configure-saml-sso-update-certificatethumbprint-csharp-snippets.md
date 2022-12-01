---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ServicePrincipal
{
	PreferredTokenSigningKeyThumbprint = "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10",
};
var result = await graphClient.ServicePrincipals["servicePrincipal-id"].PatchAsync(requestBody);


```