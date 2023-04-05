---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChecklistItem()
request_body.setDisplayName('Final sign-off from the team')



result = await client.me.todo.listsById('todoTaskList-id').tasksById('todoTask-id').checklistItems.post(request_body)


```