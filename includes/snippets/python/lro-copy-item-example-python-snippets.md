---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyPostRequestBody()
parent_reference = ItemReference()
parentReference.path = '/drive/root:/Documents'


request_body.parent_reference = parentReference
request_body.name = 'Copy of LargeFolder1'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').copy.post(request_body = request_body)


```