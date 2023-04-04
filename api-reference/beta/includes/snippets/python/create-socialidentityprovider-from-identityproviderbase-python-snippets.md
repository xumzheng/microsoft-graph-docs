---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityProviderBase();
request_body.set@odatatype('microsoft.graph.socialIdentityProvider');

request_body.setDisplayName('Login with Amazon');

additionalData = [
'identityProviderType' => 'Amazon', 
'clientId' => '56433757-cadd-4135-8431-2c9e3fd68ae8', 
'clientSecret' => '000000000000', 
];
request_body.setAdditionalData(additionalData);




result = await client.identity.identityProviders.post(request_body);


```