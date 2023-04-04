---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = FederationConfiguration();
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
request_body.setDomains(domainsArray);


'signingCertificate' => 'MIIDADCCAeigAwIBAgIQEX41y8r6', 
];
request_body.setAdditionalData(additionalData);




await client.directory().federationConfigurationsById('identityProviderBase-id').post(request_body);


```