---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RestorePostRequestBody()
parent_reference = ItemReference()
parentReference.id = 'String'


request_body.parent_reference = parentReference
request_body.name = 'String'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').restore.post(request_body = request_body)


```