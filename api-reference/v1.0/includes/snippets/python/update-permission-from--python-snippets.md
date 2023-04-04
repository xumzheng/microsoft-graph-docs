---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Permission()
request_body.setRoles(['read', ])



result = await client.sitesById('site-id').permissionsById('permission-id').patch(request_body)


```