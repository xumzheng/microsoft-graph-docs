---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetDataPostRequestBody()
request_body.sourceData = 'sourceData-value'

request_body.seriesBy = 'seriesBy-value'




await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.worksheets_by_id('workbookWorksheet-id').charts_by_id('workbookChart-id').setData.post(request_body = request_body)


```