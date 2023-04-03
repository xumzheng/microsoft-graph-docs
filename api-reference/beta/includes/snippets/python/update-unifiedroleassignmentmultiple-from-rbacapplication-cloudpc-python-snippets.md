---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleAssignmentMultiple();
requestBody.setDisplayName('NewName');

requestBody.setDescription('A new roleAssignment');



result = await client.roleManagement().cloudPC().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').patch(requestBody);


```