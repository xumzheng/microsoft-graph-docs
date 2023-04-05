---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentMultiple()
request_body.set@odatatype('#microsoft.graph.unifiedRoleAssignmentMultiple')

request_body.setDisplayName('My test role assignment 1')

request_body.setRoleDefinitionId('c2cf284d-6c41-4e6b-afac-4b80928c9034')

request_body.setPrincipalIds(['f8ca5a85-489a-49a0-b555-0a6d81e56f0d', 'c1518aa9-4da5-4c84-a902-a31404023890', ])

request_body.setAppScopeIds(['allDevices', ])



result = await client.roleManagement.deviceManagement.roleAssignments.post(request_body)


```