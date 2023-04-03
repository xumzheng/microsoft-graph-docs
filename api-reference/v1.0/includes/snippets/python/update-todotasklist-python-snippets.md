---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TodoTaskList();
requestBody.setDisplayName('Vacation Plan');



requestResult = graphServiceClient.me().todo().listsById('todoTaskList-id').patch(requestBody);


```