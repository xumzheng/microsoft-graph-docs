---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc')



await client.directoryRoles._by_id('directoryRole-id').members.ref.post(request_body)


```