---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnifiedRoleAssignmentMultiple();
request_body.setDisplayName('NewName');

request_body.setDescription('A new roleAssignment');



result = await client.roleManagement().cloudPC().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').patch(request_body);


```