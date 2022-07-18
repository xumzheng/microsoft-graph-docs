---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AuthenticationMethodConfiguration
{
	@odata.type = "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
	AdditionalData = new()
	{
		{"isUsableOnce", true},
	}
};
await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["authenticationMethodConfiguration-id"].PatchAsync(requestBody);


```