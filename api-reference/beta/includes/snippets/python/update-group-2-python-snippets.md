---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
assignedLabelsAssignedLabel1 = AssignedLabel()
assignedLabelsAssignedLabel1.setLabelId('45cd0c48-c540-4358-ad79-a3658cdc5b88')


assignedLabelsArray []= assignedLabelsAssignedLabel1;
request_body.setAssignedLabels(assignedLabelsArray)




result = await client.groupsby_id('group-id').patch(request_body)


```