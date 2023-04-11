---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPasswordPostRequestBody()
passwordCredential = PasswordCredential()
passwordCredential.displayName = 'Password friendly name'


request_body.passwordCredential = passwordCredential


request_configuration = AddPasswordRequestBuilderPostRequestConfiguration(
)


result = await client.applications_by_id('application-id').addPassword.post(request_body = request_body)


```