---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.account_enabled = True

request_body.displayName = 'MyTestUser1'

request_body.mailNickname = 'MyTestUser1'

request_body.userPrincipalName = 'MyTestUser1@contoso.com'

password_profile = PasswordProfile()
passwordProfile.force_change_password_next_sign_in = True

passwordProfile.password = 'Contoso1234'


request_body.password_profile = passwordProfile



result = await client.users.post(request_body = request_body)


```