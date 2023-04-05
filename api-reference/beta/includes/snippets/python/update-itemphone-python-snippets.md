---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPhone()
request_body.setType(PhoneType('other'))



result = await client.usersby_id('user-id').profile.phonesby_id('itemPhone-id').patch(request_body)


```