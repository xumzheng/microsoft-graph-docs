---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = $refPatchRequestBody();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test', 
'@odata.type' => '#microsoft.graph.identityProvider', 
];
requestBody.setAdditionalData(additionalData);




graphServiceClient.identity().b2xUserFlowsById('b2xIdentityUserFlow-id').userFlowIdentityProviders().ref().patch(requestBody);


```