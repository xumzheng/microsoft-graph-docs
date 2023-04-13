---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookWorksheet()
request_body.position = 99

request_body.name = 'name-value'

request_body.visibility = 'visibility-value'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.worksheets_by_id('workbookWorksheet-id').patch(request_body = request_body)


```