---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateLinkPostRequestBody()
request_body.type = 'embed'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').createLink.post(request_body = request_body)


```