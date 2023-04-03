---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = User();
requestBody.setAccountEnabled(true);

requestBody.setDisplayName('Requestor1');

requestBody.setMailNickname('Requestor1');

requestBody.setUserPrincipalName('Requestor1@contoso.onmicrosoft.com');

passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(true);

passwordProfile.setPassword('Contoso1234');


requestBody.setPasswordProfile($passwordProfile);


requestResult = graphServiceClient.users().post(requestBody);


```