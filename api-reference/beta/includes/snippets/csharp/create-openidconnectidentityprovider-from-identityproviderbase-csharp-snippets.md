---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProviderBase
{
	@odata.type = "microsoft.graph.openIdConnectIdentityProvider",
	DisplayName = "Login with the Contoso identity provider",
	AdditionalData = new()
	{
		{"clientId", "56433757-cadd-4135-8431-2c9e3fd68ae8"},
		{"clientSecret", "12345"},
		{"domainHint", "mycustomoidc"},
		{"metadataUrl", "https://mycustomoidc.com/.well-known/openid-configuration"},
		{"responseMode", "form_post"},
		{"responseType", "code"},
		{"scope", "openid"},
	}
};
var result = await graphClient.Identity.IdentityProviders.PostAsync(requestBody);


```