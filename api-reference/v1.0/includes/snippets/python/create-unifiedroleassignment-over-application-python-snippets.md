---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignment()
request_body.@odatatype = '#microsoft.graph.unifiedRoleAssignment'

request_body.principalId = '6b937a9d-c731-465b-a844-2d5b5368c161'

request_body.roleDefinitionId = '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3'

request_body.directoryScopeId = '/661e1310-bd76-4795-89a7-8f3c8f855bfc'



request_configuration = RoleAssignmentsRequestBuilderPostRequestConfiguration(
)


result = await client.roleManagement.directory.roleAssignments.post(request_body = request_body)


```