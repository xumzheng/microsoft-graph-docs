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
request_body.additionaldata(additionalData)





await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userFlowIdentityProviders_by_id('identityProviderBase-id').patch(request_body = request_body)


```