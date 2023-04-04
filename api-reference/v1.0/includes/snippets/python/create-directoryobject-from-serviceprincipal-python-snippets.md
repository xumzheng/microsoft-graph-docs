---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/directoryObjects/{id}')



await client.servicePrincipalsById('servicePrincipal-id').owners.ref.post(request_body)


```