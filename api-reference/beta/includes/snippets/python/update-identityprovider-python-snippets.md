---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProvider()
request_body.setClientSecret('1111111111111')



result = await client.identityProvidersById('identityProvider-id').patch(request_body)


```