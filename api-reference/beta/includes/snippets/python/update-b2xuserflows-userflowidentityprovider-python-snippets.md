---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $refPatchRequestBody()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test', 
'@odata.type' => '#microsoft.graph.identityProvider', 
];
request_body.setAdditionalData(additionalData)




await client.identity.b2xUserFlowsby_id('b2xIdentityUserFlow-id').userFlowIdentityProviders.ref.patch(request_body)


```