---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TodoTask();
dueDateTime = DateTimeTimeZone();
dueDateTime.setDateTime('2020-07-25T16:00:00');

dueDateTime.setTimeZone('Eastern Standard Time');


request_body.setDueDateTime($dueDateTime);


result = await client.me.todo.listsById('todoTaskList-id').tasksById('todoTask-id').patch(request_body);


```