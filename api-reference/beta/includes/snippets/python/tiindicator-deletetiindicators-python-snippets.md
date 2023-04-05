---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeleteTiIndicatorsPostRequestBody()
request_body.setValue(['id-value1', 'id-value2', ])



result = await client.security.tiIndicators.deleteTiIndicators.post(request_body)


```