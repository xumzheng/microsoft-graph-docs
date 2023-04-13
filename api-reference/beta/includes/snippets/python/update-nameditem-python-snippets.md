---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookNamedItem()
request_body.type = 'type-value'

request_body.scope = 'scope-value'

request_body.comment = 'comment-value'

value = Json()

request_body.value = value
request_body.visible = True




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.names_by_id('workbookNamedItem-id').patch(request_body = request_body)


```