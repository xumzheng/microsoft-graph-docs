---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityProvider();
additionalData = [
'responseType' => 'id_token', 
];
requestBody.setAdditionalData(additionalData);




result = await client.identityProvidersById('identityProvider-id').patch(requestBody);


```