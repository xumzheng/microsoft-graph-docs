---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChecklistItem();
requestBody.setDisplayName('buy cake');



result = await client.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').checklistItemsById('checklistItem-id').patch(requestBody);


```