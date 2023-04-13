---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalculatePostRequestBody()
request_body.calculationType = 'calculationType-value'




await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.application.calculate.post(request_body = request_body)


```