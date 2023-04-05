---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH', 
];
request_body.setAdditionalData(additionalData)




await client.identity.b2xUserFlowsById('b2xIdentityUserFlow-id').identityProvidersById('identityProvider-id').post(request_body)


```