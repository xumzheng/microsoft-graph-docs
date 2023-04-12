---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignment()
request_body.@odatatype = '#microsoft.graph.unifiedRoleAssignment'

request_body.roleDefinitionId = '58a13ea3-c632-46ae-9ee0-9c0d43cd7f3d'

request_body.principalId = 'f8ca5a85-489a-49a0-b555-0a6d81e56f0d'

request_body.directoryScopeId = '/attributeSets/Engineering'




result = await client.roleManagement.directory.roleAssignments.post(request_body = request_body)


```