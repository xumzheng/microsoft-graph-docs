---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ServicePrincipal();
requestBody.setPreferredTokenSigningKeyThumbprint('A7D3C4626B8A84FDA868CCC67D274D402FFD0A10');



result = await client.servicePrincipalsById('servicePrincipal-id').patch(requestBody);


```