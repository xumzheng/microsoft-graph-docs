---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
passwordProfile = PasswordProfile()
passwordProfile.forceChangePasswordNextSignIn = false

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.passwordProfile = passwordProfile



result = await client.users_by_id('user-id').patch(request_body = request_body)


```