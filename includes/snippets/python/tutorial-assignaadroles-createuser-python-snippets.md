---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = User();
requestBody.setAccountEnabled(true);

requestBody.setDisplayName('Aline Dupuy');

requestBody.setMailNickname('AlineD');

requestBody.setUserPrincipalName('AlineD@Contoso.com');

passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(true);

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


requestBody.setPasswordProfile($passwordProfile);


requestResult = graphServiceClient.users().post(requestBody);


```