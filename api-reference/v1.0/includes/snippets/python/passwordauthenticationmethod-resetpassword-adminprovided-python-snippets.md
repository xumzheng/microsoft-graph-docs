---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ResetPasswordPostRequestBody()
request_body.setNewPassword('Cuyo5459')



result = await client.users._by_id('user-id').authentication.methods._by_id('authenticationMethod-id').resetPassword.post(request_body)


```