---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = User();
requestBody.setAccountEnabled(true);

requestBody.setDisplayName('Adele Vance');

requestBody.setMailNickname('AdeleV');

requestBody.setUserPrincipalName('AdeleV@contoso.onmicrosoft.com');

passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(true);

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


requestBody.setPasswordProfile($passwordProfile);


requestResult = graphServiceClient.users().post(requestBody);


```