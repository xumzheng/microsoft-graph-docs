---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TodoTaskList();
requestBody.setDisplayName('Vacation Plan');



result = awaitclient.me().todo().listsById('todoTaskList-id').patch(requestBody);


```