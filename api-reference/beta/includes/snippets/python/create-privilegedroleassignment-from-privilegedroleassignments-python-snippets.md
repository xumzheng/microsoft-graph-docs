---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedRoleAssignment()
request_body.userId = 'userId-value'

request_body.roleId = 'roleId-value'




result = await client.privilegedRoleAssignments.post(request_body = request_body)


```