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

request_body.userPrincipalName = 'AdeleV@contoso.com'

passwordProfile = PasswordProfile()
passwordProfile.forceChangePasswordNextSignIn = false

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.passwordProfile = passwordProfile
additionalData = [
'extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker' => 'JobGroupN', 
];
request_body.additionaldata(additionalData)





result = await client.users.post(request_body = request_body)


```