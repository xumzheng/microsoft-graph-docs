---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
password_profile = PasswordProfile()
passwordProfile.force_change_password_next_sign_in = True

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.password_profile = passwordProfile



result = await client.users_by_id('user-id').patch(request_body = request_body)


```