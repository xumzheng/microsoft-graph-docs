---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityProvider();
requestBody.set@odatatype('microsoft.graph.openIdConnectProvider');

requestBody.setName('Login with the Contoso identity provider');

requestBody.setType('OpenIDConnect');

requestBody.setClientId('56433757-cadd-4135-8431-2c9e3fd68ae8');

requestBody.setClientSecret('12345');

additionalData = [
'claimsMapping' => requestBody = ClaimsMapping();
		requestBody.setUserId('myUserId');

		requestBody.setGivenName('myGivenName');

		requestBody.setSurname('mySurname');

		requestBody.setEmail('myEmail');

		requestBody.setDisplayName('myDisplayName');


requestBody.setClaimsMapping($claimsMapping);

'domainHint' => 'mycustomoidc', 
'metadataUrl' => 'https://mycustomoidc.com/.well-known/openid-configuration', 
'responseMode' => 'form_post', 
'responseType' => 'code', 
'scope' => 'openid', 
];
requestBody.setAdditionalData(additionalData);




result = await client.identityProviders().post(requestBody);


```