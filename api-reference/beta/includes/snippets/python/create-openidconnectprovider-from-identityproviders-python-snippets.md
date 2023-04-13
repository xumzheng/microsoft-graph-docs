---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
request_body.@odatatype = 'microsoft.graph.openIdConnectProvider'

request_body.name = 'Login with the Contoso identity provider'

request_body.type = 'OpenIDConnect'

request_body.clientId = '56433757-cadd-4135-8431-2c9e3fd68ae8'

request_body.clientSecret = '12345'

additionalData = [
'claimsMapping' => request_body = ClaimsMapping()
		request_body.userId = 'myUserId'

		request_body.givenName = 'myGivenName'

		request_body.surname = 'mySurname'

		request_body.email = 'myEmail'

		request_body.displayName = 'myDisplayName'


request_body.claimsMapping = claimsMapping

'domainHint' => 'mycustomoidc', 
'metadataUrl' => 'https://mycustomoidc.com/.well-known/openid-configuration', 
'responseMode' => 'form_post', 
'responseType' => 'code', 
'scope' => 'openid', 
];
request_body.additionaldata(additionalData)





result = await client.identityProviders.post(request_body = request_body)


```