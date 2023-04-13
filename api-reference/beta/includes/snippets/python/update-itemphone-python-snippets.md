---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPhone()
request_body.Type(PhoneType('other'))




result = await client.users_by_id('user-id').profile.phones_by_id('itemPhone-id').patch(request_body = request_body)


```