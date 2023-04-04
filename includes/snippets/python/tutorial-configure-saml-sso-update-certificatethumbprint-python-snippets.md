---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ServicePrincipal()
request_body.setPreferredTokenSigningKeyThumbprint('A7D3C4626B8A84FDA868CCC67D274D402FFD0A10')



result = await client.servicePrincipalsById('servicePrincipal-id').patch(request_body)


```