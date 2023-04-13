---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyPostRequestBody()
parent_reference = ItemReference()
parentReference.driveId = '6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B'

parentReference.id = 'DCD0D3AD-8989-4F23-A5A2-2C086050513F'


request_body.parent_reference = parentReference
request_body.name = 'contoso plan (copy).txt'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').copy.post(request_body = request_body)


```