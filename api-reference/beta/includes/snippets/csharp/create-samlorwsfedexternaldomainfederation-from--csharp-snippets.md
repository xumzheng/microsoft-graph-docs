---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityProviderBase-idRequestBody
{
	AdditionalData = new()
	{
		{"@odata.type", "microsoft.graph.samlOrWsFedExternalDomainFederation"},
		{"issuerUri", "https://contoso.com/issuerUri"},
		{"displayName", "contoso display name"},
		{"metadataExchangeUri", "https://contoso.com/metadataExchangeUri"},
		{"passiveSignInUri", "https://contoso.com/signin"},
		{"preferredAuthenticationProtocol", "wsFed"},
		{"domains", new List<Object>
		{
		}
		{"signingCertificate", "MIIDADCCAeigAwIBAgIQEX41y8r6"},
	}
};
await graphClient.Directory.FederationConfigurations["identityProviderBase-id"].PostAsync(requestBody);


```