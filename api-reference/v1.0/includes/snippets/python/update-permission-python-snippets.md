---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Permission()
request_body.Roles(['read', ])




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').permissions_by_id('permission-id').patch(request_body = request_body)


```