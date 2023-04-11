---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TemporaryAccessPassAuthenticationMethod()
request_body.startDateTime = DateTime('2022-06-05T00:00:00.000Z')

request_body.lifetimeInMinutes = 60

request_body.isUsableOnce = false




result = await client.users_by_id('user-id').authentication.temporaryAccessPassMethods.post(request_body = request_body)


```