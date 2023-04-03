---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EmailAuthenticationMethod();
requestBody.setEmailAddress('kim@contoso.com');



result = await client.usersById('user-id').authentication().emailMethods().post(requestBody);


```