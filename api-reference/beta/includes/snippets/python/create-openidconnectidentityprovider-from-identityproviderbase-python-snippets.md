---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityProviderBase();
request_body.set@odatatype('microsoft.graph.openIdConnectIdentityProvider');

request_body.setDisplayName('Login with the Contoso identity provider');

additionalData = [
'clientId' => '56433757-cadd-4135-8431-2c9e3fd68ae8', 
'clientSecret' => '12345', 
'claimsMapping' => request_body = ClaimsMapping();
		request_body.setUserId('myUserId');

		request_body.setGivenName('myGivenName');

		request_body.setSurname('mySurname');

		request_body.setEmail('myEmail');

		request_body.setDisplayName('myDisplayName');


request_body.setClaimsMapping($claimsMapping);

'domainHint' => 'mycustomoidc', 
'metadataUrl' => 'https://mycustomoidc.com/.well-known/openid-configuration', 
'responseMode' => 'form_post', 
'responseType' => 'code', 
'scope' => 'openid', 
];
request_body.setAdditionalData(additionalData);




result = await client.identity.identityProviders.post(request_body);


```