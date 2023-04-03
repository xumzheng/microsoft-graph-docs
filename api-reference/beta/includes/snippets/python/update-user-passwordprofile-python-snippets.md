---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = User();
passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(true);

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


requestBody.setPasswordProfile($passwordProfile);


result = await client.usersById('user-id').patch(requestBody);


```