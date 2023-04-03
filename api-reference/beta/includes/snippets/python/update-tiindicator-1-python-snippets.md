---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TiIndicator();
requestBody.setDescription('description-updated');



result = await client.security().tiIndicatorsById('tiIndicator-id').patch(requestBody);


```