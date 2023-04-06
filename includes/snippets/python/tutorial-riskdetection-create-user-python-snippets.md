---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.setAccountEnabled(true)

request_body.setDisplayName('MyTestUser1')

request_body.setMailNickname('MyTestUser1')

request_body.setUserPrincipalName('MyTestUser1@contoso.com')

passwordProfile = PasswordProfile()
passwordProfile.setForceChangePasswordNextSignIn(true)

passwordProfile.setPassword('Contoso1234')


request_body.setPasswordProfile($passwordProfile)

request_config = UsersRequestBuilderPostRequestConfiguration(
request_config = UsersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.users.post(request_body, headers=)


```