---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = FederationConfiguration();
additionalData = [
'@odata.type' => 'microsoft.graph.samlOrWsFedExternalDomainFederation', 
'issuerUri' => 'https://contoso.com/issuerUri', 
'displayName' => 'contoso display name', 
'metadataExchangeUri' => 'https://contoso.com/metadataExchangeUri', 
'passiveSignInUri' => 'https://contoso.com/signin', 
'preferredAuthenticationProtocol' => 'wsFed', 
'domains' => domains1 = ();
		domains1.set@odatatype('microsoft.graph.externalDomainName');

		domains1.setId('contoso.com');


domainsArray []= domains1;
requestBody.setDomains(domainsArray);


'signingCertificate' => 'MIIDADCCAeigAwIBAgIQEX41y8r6', 
];
requestBody.setAdditionalData(additionalData);




await client.directory().federationConfigurationsById('identityProviderBase-id').post(requestBody);


```