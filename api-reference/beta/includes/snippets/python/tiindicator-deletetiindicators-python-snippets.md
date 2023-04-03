---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = DeleteTiIndicatorsPostRequestBody();
requestBody.setValue(['id-value1', 'id-value2', ]);



result = awaitclient.security().tiIndicators().deleteTiIndicators().post(requestBody);


```