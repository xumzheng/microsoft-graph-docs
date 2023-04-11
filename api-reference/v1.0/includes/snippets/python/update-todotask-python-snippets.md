---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TodoTask()
dueDateTime = DateTimeTimeZone()
dueDateTime.dateTime = '2020-07-25T16:00:00'

dueDateTime.timeZone = 'Eastern Standard Time'


request_body.dueDateTime = dueDateTime



result = await client.me.todo.lists_by_id('todoTaskList-id').tasks_by_id('todoTask-id').patch(request_body = request_body)


```