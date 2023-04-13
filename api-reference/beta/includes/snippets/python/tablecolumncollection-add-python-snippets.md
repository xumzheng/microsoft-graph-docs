---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
index = Index()

request_body.index = index
values_json1 = Json()

valuesArray []= valuesJson1;
request_body.values(valuesArray)





result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').columns.add.post(request_body = request_body)


```