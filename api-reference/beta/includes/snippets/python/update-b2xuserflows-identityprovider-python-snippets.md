---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityProvider();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/identityProviders/{id}', 
];
requestBody.setAdditionalData(additionalData);




graphServiceClient.identity().b2xUserFlowsById('b2xIdentityUserFlow-id').identityProvidersById('identityProvider-id').post(requestBody);


```