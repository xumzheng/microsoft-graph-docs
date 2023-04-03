---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = User();
requestBody.setAccountEnabled(true);

requestBody.setDisplayName('MyTestUser1');

requestBody.setMailNickname('MyTestUser1');

requestBody.setUserPrincipalName('MyTestUser1@contoso.com');

passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(true);

passwordProfile.setPassword('Contoso1234');


requestBody.setPasswordProfile($passwordProfile);


result = await client.users().post(requestBody);


```