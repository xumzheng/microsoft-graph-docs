---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddTokenSigningCertificatePostRequestBody()
request_body.setDisplayName('CN=customDisplayName')

request_body.setEndDateTime(DateTime('2024-01-25T00:00:00Z'))



result = await client.servicePrincipals._by_id('servicePrincipal-id').addTokenSigningCertificate.post(request_body)


```