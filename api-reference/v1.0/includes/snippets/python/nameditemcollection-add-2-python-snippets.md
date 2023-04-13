---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddFormulaLocalPostRequestBody()
request_body.name = 'test7'

request_body.formula = '=SUM(Sheet2!$A$1+Sheet2!$A$2)'

request_body.comment = 'Comment for the named item'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.names.addFormulaLocal.post(request_body = request_body)


```