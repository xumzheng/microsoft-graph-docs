---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserFlowIdentityProvider()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/identity/identityProviders/{id}', 
'@odata.type' => '#microsoft.graph.identityProvider', 
];
request_body.setAdditionalData(additionalData)




await client.identity.b2cUserFlowsby_id('b2cIdentityUserFlow-id').userFlowIdentityProvidersby_id('identityProviderBase-id').patch(request_body)


```