---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PrivilegedRoleAssignment();
requestBody.setUserId('userId-value');

requestBody.setRoleId('roleId-value');



result = await client.privilegedRoleAssignments().post(requestBody);


```