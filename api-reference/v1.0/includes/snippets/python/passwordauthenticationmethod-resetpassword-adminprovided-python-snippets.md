---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ResetPasswordPostRequestBody();
requestBody.setNewPassword('Cuyo5459');



result = await client.usersById('user-id').authentication().methodsById('authenticationMethod-id').resetPassword().post(requestBody);


```