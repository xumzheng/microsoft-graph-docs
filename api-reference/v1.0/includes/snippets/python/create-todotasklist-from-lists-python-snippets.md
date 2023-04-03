---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TodoTaskList();
requestBody.setDisplayName('Travel items');



result = await client.me().todo().lists().post(requestBody);


```