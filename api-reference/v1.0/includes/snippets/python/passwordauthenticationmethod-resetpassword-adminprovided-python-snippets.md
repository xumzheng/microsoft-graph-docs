---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ResetPasswordPostRequestBody();
$requestBody.setNewPassword('Cuyo5459');



$requestResult = $graphServiceClient.usersById('user-id').authentication().methodsById('authenticationMethod-id').resetPassword().post($requestBody);


```