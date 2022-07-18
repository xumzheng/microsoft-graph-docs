---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProvider
{
	ClientSecret = "1111111111111",
};
await graphClient.IdentityProviders["identityProvider-id"].PatchAsync(requestBody);


```