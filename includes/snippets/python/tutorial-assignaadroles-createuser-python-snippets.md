---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.setAccountEnabled(true)

request_body.setDisplayName('Aline Dupuy')

request_body.setMailNickname('AlineD')

request_body.setUserPrincipalName('AlineD@Contoso.com')

passwordProfile = PasswordProfile()
passwordProfile.setForceChangePasswordNextSignIn(true)

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d')


request_body.setPasswordProfile($passwordProfile)


result = await client.users.post(request_body, headers=)


```