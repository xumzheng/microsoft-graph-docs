---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.accountEnabled = true

request_body.displayName = 'MyTestUser1'

request_body.mailNickname = 'MyTestUser1'

request_body.userPrincipalName = 'MyTestUser1@contoso.com'

passwordProfile = PasswordProfile()
passwordProfile.forceChangePasswordNextSignIn = true

passwordProfile.password = 'Contoso1234'


request_body.passwordProfile = passwordProfile


request_configuration = UsersRequestBuilderPostRequestConfiguration(
)


result = await client.users.post(request_body = request_body)


```