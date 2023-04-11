---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.accountEnabled = true

request_body.displayName = 'Adele Vance'

request_body.mailNickname = 'AdeleV'

request_body.userPrincipalName = 'AdeleV@contoso.onmicrosoft.com'

passwordProfile = PasswordProfile()
passwordProfile.forceChangePasswordNextSignIn = true

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.passwordProfile = passwordProfile


request_configuration = UsersRequestBuilderPostRequestConfiguration(
)


result = await client.users.post(request_body = request_body)


```