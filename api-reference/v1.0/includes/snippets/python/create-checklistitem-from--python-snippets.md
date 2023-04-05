---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChecklistItem()
request_body.setDisplayName('Final sign-off from the team')



result = await client.me_todo_listsby_id('todoTaskList-id')_tasksby_id('todoTask-id')_checklistItems.post(request_body)


```