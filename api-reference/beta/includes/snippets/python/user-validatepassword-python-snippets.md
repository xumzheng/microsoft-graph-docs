---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ValidatePasswordPostRequestBody();
requestBody.setPassword('1234567890');



result = await client.users().validatePassword().post(requestBody);


```