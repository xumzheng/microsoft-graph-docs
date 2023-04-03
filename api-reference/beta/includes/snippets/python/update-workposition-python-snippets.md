---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = WorkPosition();
requestBody.setIsCurrent(true);



result = awaitclient.me().profile().positionsById('workPosition-id').patch(requestBody);


```