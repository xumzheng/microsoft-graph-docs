---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentMultiple()
request_body.PrincipalIds(['0aeec2c1-fee7-4e02-b534-6f920d25b300', '2d5386a7-732f-44db-9cf8-f82dd2a1c0e0', ])



request_configuration = UnifiedRoleAssignmentMultipleRequestBuilderPatchRequestConfiguration(
)


result = await client.roleManagement.deviceManagement.roleAssignments_by_id('unifiedRoleAssignmentMultiple-id').patch(request_body = request_body)


```