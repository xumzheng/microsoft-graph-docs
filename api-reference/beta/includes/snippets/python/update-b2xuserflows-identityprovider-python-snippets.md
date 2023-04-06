---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/identityProviders/{id}', 
];
request_body.setAdditionalData(additionalData)



request_config = IdentityProviderRequestBuilderPostRequestConfiguration(
request_config = IdentityProviderRequestBuilderPostRequestConfiguration(query_params=)


await client.identity.b2xUserFlows_by_id('b2xIdentityUserFlow-id').identityProviders_by_id('identityProvider-id').post(request_body, headers=)


```