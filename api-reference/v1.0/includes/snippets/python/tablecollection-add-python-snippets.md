---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
request_body.address = 'Sheet1!A1:D5'

request_body.has_headers = True




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables.add.post(request_body = request_body)


```