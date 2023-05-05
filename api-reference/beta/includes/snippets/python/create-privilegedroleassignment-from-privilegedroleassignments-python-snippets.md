---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedRoleAssignment()
request_body.user_id = 'userId-value'

request_body.role_id = 'roleId-value'




result = await client.privileged_role_assignments.post(request_body = request_body)


```