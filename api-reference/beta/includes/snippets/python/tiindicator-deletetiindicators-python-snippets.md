---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = DeleteTiIndicatorsPostRequestBody();
requestBody.setValue(['id-value1', 'id-value2', ]);



requestResult = graphServiceClient.security().tiIndicators().deleteTiIndicators().post(requestBody);


```