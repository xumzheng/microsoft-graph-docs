---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
additionalData = [
'responseType' => 'id_token', 
];
request_body.setAdditionalData(additionalData)



request_config = IdentityProviderRequestBuilderPatchRequestConfiguration(
request_config = IdentityProviderRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identityProviders_by_id('identityProvider-id').patch(request_body, headers=)


```