---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
request_body.name = 'test5'

request_body.reference = '=Sheet1!$F$15:$N$27'

request_body.comment = 'Comment for the named item'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.names.add.post(request_body = request_body)


```