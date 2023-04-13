---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Row()
additionalData = [
'index' => 4,
];
request_body.additionaldata(additionalData)





await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').rows_by_id('workbookTableRow-id').post(request_body = request_body)


```