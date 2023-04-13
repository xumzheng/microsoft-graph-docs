---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.account_enabled = True

request_body.displayName = 'Requestor1'

request_body.mailNickname = 'Requestor1'

request_body.userPrincipalName = 'Requestor1@contoso.onmicrosoft.com'

password_profile = PasswordProfile()
passwordProfile.force_change_password_next_sign_in = True

passwordProfile.password = 'Contoso1234'


request_body.password_profile = passwordProfile



result = await client.users.post(request_body = request_body)


```