---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPasswordPostRequestBody()
passwordCredential = PasswordCredential()
passwordCredential.setDisplayName('Password friendly name')


request_body.setPasswordCredential($passwordCredential)


result = await client.applications_by_id('application-id').addPassword.post(request_body, headers=)


```