---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChecklistItem()
request_body.displayName = 'Final sign-off from the team'



request_configuration = ChecklistItemsRequestBuilderPostRequestConfiguration(
)


result = await client.me.todo.lists_by_id('todoTaskList-id').tasks_by_id('todoTask-id').checklistItems.post(request_body = request_body)


```