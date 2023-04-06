---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedRoleAssignment()
request_body.setUserId('userId-value')

request_body.setRoleId('roleId-value')


request_config = PrivilegedRoleAssignmentsRequestBuilderPostRequestConfiguration(
request_config = PrivilegedRoleAssignmentsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.privilegedRoleAssignments.post(request_body, headers=)


```