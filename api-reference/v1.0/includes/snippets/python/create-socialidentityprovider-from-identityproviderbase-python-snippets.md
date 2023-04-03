---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityProviderBase();
requestBody.set@odatatype('microsoft.graph.socialIdentityProvider');

requestBody.setDisplayName('Login with Amazon');

additionalData = [
'identityProviderType' => 'Amazon', 
'clientId' => '56433757-cadd-4135-8431-2c9e3fd68ae8', 
'clientSecret' => '000000000000', 
];
requestBody.setAdditionalData(additionalData);




result = await client.identity().identityProviders().post(requestBody);


```