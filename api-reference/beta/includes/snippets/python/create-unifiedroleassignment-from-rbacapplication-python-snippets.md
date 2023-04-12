---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignment()
request_body.@odatatype = '#microsoft.graph.unifiedRoleAssignment'

request_body.roleDefinitionId = 'c2cf284d-6c41-4e6b-afac-4b80928c9034'

request_body.principalId = 'f8ca5a85-489a-49a0-b555-0a6d81e56f0d'

request_body.directoryScopeId = '/'




result = await client.roleManagement.directory.roleAssignments.post(request_body = request_body)


```