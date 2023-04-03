---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChecklistItem();
requestBody.setDisplayName('Final sign-off from the team');



requestResult = graphServiceClient.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').checklistItems().post(requestBody);


```