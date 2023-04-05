---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UploadSecretPostRequestBody()
request_body.setUse('use-value')

request_body.setK('application-secret-to-be-uploaded')

request_body.setNbf(1508969811)

request_body.setExp(1508973711)



result = await client.trustFramework.keySets_by_id('trustFrameworkKeySet-id').uploadSecret.post(request_body)


```