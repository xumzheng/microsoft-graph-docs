---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = WorkPosition();
requestBody.setIsCurrent(true);



result = await client.me().profile().positionsById('workPosition-id').patch(requestBody);


```