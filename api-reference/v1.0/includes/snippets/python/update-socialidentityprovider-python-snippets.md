---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProviderBase()
request_body.set@odatatype('#microsoft.graph.socialIdentityProvider')

additionalData = [
'clientSecret' => '1111111111111', 
];
request_body.setAdditionalData(additionalData)




result = await client.identity.identityProvidersby_id('identityProviderBase-id').patch(request_body)


```