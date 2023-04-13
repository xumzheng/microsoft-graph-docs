---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookChartFont()
request_body.bold = True

request_body.color = 'color-value'

request_body.italic = True

request_body.name = 'name-value'

request_body.size = 99

request_body.underline = 'underline-value'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.worksheets_by_id('workbookWorksheet-id').charts_by_id('workbookChart-id').axes.valueAxis.format.font.patch(request_body = request_body)


```