---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TodoTaskList();
requestBody.setDisplayName('Vacation Plan');



result = await client.me().todo().listsById('todoTaskList-id').patch(requestBody);


```