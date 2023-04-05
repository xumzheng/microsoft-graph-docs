---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChecklistItem()
request_body.setDisplayName('buy cake')



result = await client.me.todo.listsby_id('todoTaskList-id').tasksby_id('todoTask-id').checklistItemsby_id('checklistItem-id').patch(request_body)


```