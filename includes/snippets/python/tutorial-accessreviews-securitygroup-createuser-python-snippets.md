---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.account_enabled = True

request_body.displayName = 'Adele Vance'

request_body.mailNickname = 'AdeleV'

request_body.userPrincipalName = 'AdeleV@Contoso.com'

password_profile = PasswordProfile()
passwordProfile.force_change_password_next_sign_in = True

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.password_profile = passwordProfile



result = await client.users.post(request_body = request_body)


```