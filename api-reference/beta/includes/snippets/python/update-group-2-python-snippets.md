---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Group();
assignedLabelsAssignedLabel1 = AssignedLabel();
assignedLabelsAssignedLabel1.setLabelId('45cd0c48-c540-4358-ad79-a3658cdc5b88');


assignedLabelsArray []= assignedLabelsAssignedLabel1;
requestBody.setAssignedLabels(assignedLabelsArray);




result = awaitclient.groupsById('group-id').patch(requestBody);


```