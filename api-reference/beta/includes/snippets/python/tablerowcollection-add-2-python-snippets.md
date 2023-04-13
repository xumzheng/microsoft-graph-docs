---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
request_body.index=null

request_body.Values([[1,2,3,],[4,5,6,],])




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').rows.add.post(request_body = request_body)


```