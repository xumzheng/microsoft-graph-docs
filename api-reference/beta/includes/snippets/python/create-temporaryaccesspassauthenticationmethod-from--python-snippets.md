---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TemporaryAccessPassAuthenticationMethod()
request_body.setStartDateTime(DateTime('2022-06-05T00:00:00.000Z'))

request_body.setLifetimeInMinutes(60)

request_body.setIsUsableOnce(false)



result = await client.usersById('user-id').authentication.temporaryAccessPassMethods.post(request_body)


```