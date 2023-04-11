---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddKeyPostRequestBody()
keyCredential = KeyCredential()
keyCredential.type = 'AsymmetricX509Cert'

keyCredential.usage = 'Verify'

KeyCredential.Key(base64_decode('MIIDYDCCAki...'))


request_body.keyCredential = keyCredential
request_body.passwordCredential=null

request_body.proof = 'eyJ0eXAiOiJ...'



request_configuration = AddKeyRequestBuilderPostRequestConfiguration(
)


result = await client.servicePrincipals_by_id('servicePrincipal-id').addKey.post(request_body = request_body)


```