---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityProvider();
additionalData = [
'responseType' => 'id_token', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.identityProvidersById('identityProvider-id').patch(requestBody);


```