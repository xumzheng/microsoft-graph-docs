---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityProvider();
additionalData = [
'responseType' => 'id_token', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.identityProvidersById('identityProvider-id').patch(requestBody);


```