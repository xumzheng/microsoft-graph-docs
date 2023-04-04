---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = $refDeleteRequestBody();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/directoryObjects/{id}', 
];
request_body.setAdditionalData(additionalData);




await client.servicePrincipalsById('servicePrincipal-id').ownersById('directoryObject-id').ref.delete(request_body);


```