---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = User();
requestBody.setAccountEnabled(true);

requestBody.setDisplayName('Adele Vance');

requestBody.setMailNickname('AdeleV');

requestBody.setUserPrincipalName('AdeleV@contoso.com');

passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(false);

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


requestBody.setPasswordProfile($passwordProfile);
additionalData = [
'extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker' => 'JobGroupN', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.users().post(requestBody);


```