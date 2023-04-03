---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = DeleteTiIndicatorsByExternalIdPostRequestBody();
requestBody.setValue(['externalId-value1', 'externalId-value2', ]);



requestResult = graphServiceClient.security().tiIndicators().deleteTiIndicatorsByExternalId().post(requestBody);


```