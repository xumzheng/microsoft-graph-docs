---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ValidatePasswordPostRequestBody()
request_body.setPassword('1234567890')



result = await client.users_validatePassword.post(request_body)


```