---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ValidatePasswordPostRequestBody();
requestBody.setPassword('1234567890');



requestResult = graphServiceClient.users().validatePassword().post(requestBody);


```