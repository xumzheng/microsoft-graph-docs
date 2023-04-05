---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.setAccountEnabled(true)

request_body.setDisplayName('Adele Vance')

request_body.setMailNickname('AdeleV')

request_body.setUserPrincipalName('AdeleV@contoso.com')

passwordProfile = PasswordProfile()
passwordProfile.setForceChangePasswordNextSignIn(false)

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d')


request_body.setPasswordProfile($passwordProfile)
additionalData = [
'extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker' => 'JobGroupN', 
];
request_body.setAdditionalData(additionalData)




result = await client.users.post(request_body)


```