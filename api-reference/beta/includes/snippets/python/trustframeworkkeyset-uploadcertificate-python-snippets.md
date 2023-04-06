---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UploadCertificatePostRequestBody()
request_body.setKey('key-value')



result = await client.trustFramework.keySets_by_id('trustFrameworkKeySet-id').uploadCertificate.post(request_body, headers=)


```