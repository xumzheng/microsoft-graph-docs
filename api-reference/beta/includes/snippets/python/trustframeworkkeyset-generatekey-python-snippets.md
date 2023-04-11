---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GenerateKeyPostRequestBody()
request_body.use = 'sig'

request_body.kty = 'RSA'

request_body.nbf = 1508969811

request_body.exp = 1508969811




result = await client.trustFramework.keySets_by_id('trustFrameworkKeySet-id').generateKey.post(request_body = request_body)


```