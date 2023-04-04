---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityProvider();
request_body.set@odatatype('microsoft.graph.openIdConnectProvider');

request_body.setName('Login with the Contoso identity provider');

request_body.setType('OpenIDConnect');

request_body.setClientId('56433757-cadd-4135-8431-2c9e3fd68ae8');

request_body.setClientSecret('12345');

additionalData = [
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




result = await client.identityProviders().post(request_body);


```