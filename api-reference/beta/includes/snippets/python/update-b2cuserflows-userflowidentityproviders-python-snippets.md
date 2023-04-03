---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserFlowIdentityProvider();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/identity/identityProviders/{id}', 
'@odata.type' => '#microsoft.graph.identityProvider', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userFlowIdentityProvidersById('identityProviderBase-id').patch(requestBody);


```