---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.BusinessPhones(['+1 425 555 0109', ])

request_body.officeLocation = '18/2111'




result = await client.users_by_id('user-id').patch(request_body = request_body)


```