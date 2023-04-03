---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TiIndicator();
requestBody.setDescription('description-updated');



requestResult = graphServiceClient.security().tiIndicatorsById('tiIndicator-id').patch(requestBody);


```