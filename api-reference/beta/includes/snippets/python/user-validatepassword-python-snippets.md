---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ValidatePasswordPostRequestBody();
requestBody.setPassword('1234567890');



result = awaitclient.users().validatePassword().post(requestBody);


```