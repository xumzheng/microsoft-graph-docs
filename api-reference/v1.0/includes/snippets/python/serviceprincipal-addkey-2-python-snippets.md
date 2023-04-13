---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddKeyPostRequestBody()
key_credential = KeyCredential()
keyCredential.type = 'X509CertAndPassword'

keyCredential.usage = 'Sign'

KeyCredential.Key(base64_decode('MIIDYDCCAki...'))


request_body.key_credential = keyCredential
password_credential = PasswordCredential()
passwordCredential.secretText = 'MKTr0w1...'


request_body.password_credential = passwordCredential
request_body.proof = 'eyJ0eXAiOiJ...'




result = await client.servicePrincipals_by_id('servicePrincipal-id').addKey.post(request_body = request_body)


```