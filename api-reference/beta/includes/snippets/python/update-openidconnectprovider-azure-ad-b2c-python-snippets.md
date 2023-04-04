---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityProvider();
additionalData = [
'responseType' => 'id_token', 
];
request_body.setAdditionalData(additionalData);




result = await client.identityProvidersById('identityProvider-id').patch(request_body);


```