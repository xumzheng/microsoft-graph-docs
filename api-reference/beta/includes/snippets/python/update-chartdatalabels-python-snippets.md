---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookChartDataLabels()
request_body.position = 'position-value'

request_body.show_value = True

request_body.show_series_name = True

request_body.show_category_name = True

request_body.show_legend_key = True




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.worksheets_by_id('workbookWorksheet-id').charts_by_id('workbookChart-id').dataLabels.patch(request_body = request_body)


```