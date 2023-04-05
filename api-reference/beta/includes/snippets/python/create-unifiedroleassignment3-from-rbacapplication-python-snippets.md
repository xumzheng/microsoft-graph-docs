---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignment()
request_body.setPrincipalId('679a9213-c497-48a4-830a-8d3d25d94ddc')

request_body.setRoleDefinitionId('ae79f266-94d4-4dab-b730-feca7e132178')

request_body.setAppScopeId('/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997')



result = await client.roleManagement_entitlementManagement_roleAssignments.post(request_body)


```