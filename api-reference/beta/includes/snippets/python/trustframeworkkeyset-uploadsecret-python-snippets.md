---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UploadSecretPostRequestBody()
request_body.use = 'use-value'

request_body.k = 'application-secret-to-be-uploaded'

request_body.nbf = 1508969811

request_body.exp = 1508973711




result = await client.trustFramework.keySets_by_id('trustFrameworkKeySet-id').uploadSecret.post(request_body = request_body)


```