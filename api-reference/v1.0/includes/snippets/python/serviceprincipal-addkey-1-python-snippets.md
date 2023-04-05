---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddKeyPostRequestBody()
keyCredential = KeyCredential()
keyCredential.setType('AsymmetricX509Cert')

keyCredential.setUsage('Verify')

KeyCredential.setKey(base64_decode('MIIDYDCCAki...'))


request_body.setKeyCredential($keyCredential)
request_body.setPasswordCredential(null)

request_body.setProof('eyJ0eXAiOiJ...')



result = await client.servicePrincipalsby_id('servicePrincipal-id')_addKey.post(request_body)


```