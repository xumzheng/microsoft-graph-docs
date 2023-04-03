---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DeleteTiIndicatorsByExternalIdPostRequestBody();
requestBody.setValue(['externalId-value1', 'externalId-value2', ]);



result = await client.security().tiIndicators().deleteTiIndicatorsByExternalId().post(requestBody);


```