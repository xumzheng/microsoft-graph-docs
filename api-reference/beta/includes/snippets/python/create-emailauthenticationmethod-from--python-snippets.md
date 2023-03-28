---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EmailAuthenticationMethod();
$requestBody.setEmailAddress('kim@contoso.com');



$requestResult = $graphServiceClient.usersById('user-id').authentication().emailMethods().post($requestBody);


```