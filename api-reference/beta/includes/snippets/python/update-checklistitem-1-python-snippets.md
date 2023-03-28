---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChecklistItem();
$requestBody.setDisplayName('buy cake');



$requestResult = $graphServiceClient.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').checklistItemsById('checklistItem-id').patch($requestBody);


```