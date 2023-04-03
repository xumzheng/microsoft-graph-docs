---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = User();
passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(false);

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


requestBody.setPasswordProfile($passwordProfile);


result = awaitclient.usersById('user-id').patch(requestBody);


```