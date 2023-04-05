---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddKeyPostRequestBody()
keyCredential = KeyCredential()
keyCredential.setType('X509CertAndPassword')

keyCredential.setUsage('Sign')

KeyCredential.setKey(base64_decode('MIIDYDCCAki...'))


request_body.setKeyCredential($keyCredential)
passwordCredential = PasswordCredential()
passwordCredential.setSecretText('MKTr0w1...')


request_body.setPasswordCredential($passwordCredential)
request_body.setProof('eyJ0eXAiOiJ...')



result = await client.servicePrincipals_by_id('servicePrincipal-id').addKey.post(request_body)


```