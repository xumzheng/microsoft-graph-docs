---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityProviderBase();
requestBody.set@odatatype('microsoft.graph.openIdConnectIdentityProvider');

requestBody.setDisplayName('Login with the Contoso identity provider');

additionalData = [
'clientId' => '56433757-cadd-4135-8431-2c9e3fd68ae8', 
'clientSecret' => '12345', 
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




requestResult = graphServiceClient.identity().identityProviders().post(requestBody);


```