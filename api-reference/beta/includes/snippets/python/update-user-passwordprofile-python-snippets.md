---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
passwordProfile = PasswordProfile()
passwordProfile.setForceChangePasswordNextSignIn(true)

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d')


request_body.setPasswordProfile($passwordProfile)


result = await client.usersById('user-id').patch(request_body)


```