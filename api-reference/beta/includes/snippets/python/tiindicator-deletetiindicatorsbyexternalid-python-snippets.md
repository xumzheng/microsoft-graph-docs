---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeleteTiIndicatorsByExternalIdPostRequestBody()
request_body.setValue(['externalId-value1', 'externalId-value2', ])



result = await client.security.tiIndicators.deleteTiIndicatorsByExternalId.post(request_body, headers=)


```