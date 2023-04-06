---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.setAccountEnabled(true)

request_body.setDisplayName('Requestor1')

request_body.setMailNickname('Requestor1')

request_body.setUserPrincipalName('Requestor1@contoso.onmicrosoft.com')

passwordProfile = PasswordProfile()
passwordProfile.setForceChangePasswordNextSignIn(true)

passwordProfile.setPassword('Contoso1234')


request_body.setPasswordProfile($passwordProfile)


result = await client.users.post(request_body, headers=)


```