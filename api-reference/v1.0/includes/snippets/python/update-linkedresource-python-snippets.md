---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = LinkedResource();
requestBody.set@odatatype('#microsoft.graph.linkedResource');

requestBody.setWebUrl('http://microsoft.com');

requestBody.setApplicationName('Microsoft');

requestBody.setDisplayName('Microsoft');



requestResult = graphServiceClient.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').linkedResourcesById('linkedResource-id').patch(requestBody);


```