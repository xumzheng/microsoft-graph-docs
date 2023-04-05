---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Permission()
request_body.setRoles(['read', ])



result = await client.sites._by_id('site-id').permissions._by_id('permission-id').patch(request_body)


```