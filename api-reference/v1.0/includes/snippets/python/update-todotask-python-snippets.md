---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TodoTask();
dueDateTime = DateTimeTimeZone();
dueDateTime.setDateTime('2020-07-25T16:00:00');

dueDateTime.setTimeZone('Eastern Standard Time');


requestBody.setDueDateTime($dueDateTime);


result = awaitclient.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').patch(requestBody);


```