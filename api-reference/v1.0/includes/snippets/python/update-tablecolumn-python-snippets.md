---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookTableColumn()
request_body.name = 'name-value'

request_body.index = 99

request_body.values = 'values-value'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').columns_by_id('workbookTableColumn-id').patch(request_body = request_body)


```