---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleAssignmentMultiple();
requestBody.setPrincipalIds(['0aeec2c1-fee7-4e02-b534-6f920d25b300', '2d5386a7-732f-44db-9cf8-f82dd2a1c0e0', ]);



result = await client.roleManagement().deviceManagement().roleAssignmentsById('unifiedRoleAssignmentMultiple-id').patch(requestBody);


```