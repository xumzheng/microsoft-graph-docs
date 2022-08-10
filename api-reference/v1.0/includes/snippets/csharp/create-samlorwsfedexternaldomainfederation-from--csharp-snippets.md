---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new FederationConfiguration
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.type" , "microsoft.graph.samlOrWsFedExternalDomainFederation"
		},
		{
			"issuerUri" , "https://contoso.com/issuerUri"
		},
		{
			"displayName" , "contoso display name"
		},
		{
			"metadataExchangeUri" , "https://contoso.com/metadataExchangeUri"
		},
		{
			"passiveSignInUri" , "https://contoso.com/signin"
		},
		{
			"preferredAuthenticationProtocol" , "wsFed"
		},
		{
			"domains" , new List<>
			{
				new 
				{
					OdataType = "microsoft.graph.externalDomainName",
					Id = "contoso.com",
				},
			}
		},
		{
			"signingCertificate" , "MIIDADCCAeigAwIBAgIQEX41y8r6"
		},
	},
};
await graphClient.Directory.FederationConfigurations["identityProviderBase-id"].PostAsync(requestBody);


```