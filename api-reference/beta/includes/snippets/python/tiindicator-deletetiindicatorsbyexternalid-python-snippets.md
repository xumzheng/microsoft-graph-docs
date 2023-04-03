---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = DeleteTiIndicatorsByExternalIdPostRequestBody();
requestBody.setValue(['externalId-value1', 'externalId-value2', ]);



result = awaitclient.security().tiIndicators().deleteTiIndicatorsByExternalId().post(requestBody);


```