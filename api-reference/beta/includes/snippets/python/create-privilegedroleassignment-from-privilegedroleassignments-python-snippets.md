---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PrivilegedRoleAssignment();
requestBody.setUserId('userId-value');

requestBody.setRoleId('roleId-value');



requestResult = graphServiceClient.privilegedRoleAssignments().post(requestBody);


```