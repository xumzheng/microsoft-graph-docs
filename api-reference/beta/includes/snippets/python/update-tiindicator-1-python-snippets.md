---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TiIndicator();
requestBody.setDescription('description-updated');



result = awaitclient.security().tiIndicatorsById('tiIndicator-id').patch(requestBody);


```