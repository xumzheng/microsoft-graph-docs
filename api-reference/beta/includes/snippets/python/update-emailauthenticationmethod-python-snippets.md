---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EmailAuthenticationMethod();
requestBody.setEmailAddress('kim@contoso.com');



result = awaitclient.usersById('user-id').authentication().emailMethodsById('emailAuthenticationMethod-id').patch(requestBody);


```