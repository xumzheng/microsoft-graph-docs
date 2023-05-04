---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Todo_task()
due_date_time = Date_time_time_zone()
due_date_time.date_time = '2020-07-25T16:00:00'

due_date_time.time_zone = 'Eastern Standard Time'


request_body.due_date_time = due_date_time



result = await client.me.todo.lists.by_list_id('todoTaskList-id').tasks.by_task_id('todoTask-id').patch(request_body = request_body)


```