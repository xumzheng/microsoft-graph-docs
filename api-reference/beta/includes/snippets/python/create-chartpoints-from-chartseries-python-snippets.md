---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookChartPoint()



result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.worksheets_by_id('workbookWorksheet-id').charts_by_id('workbookChart-id').series_by_id('workbookChartSeries-id').points.post(request_body = request_body)


```