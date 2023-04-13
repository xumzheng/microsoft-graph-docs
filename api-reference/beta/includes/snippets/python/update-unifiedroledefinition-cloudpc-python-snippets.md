---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleDefinition()
request_body.description = 'Update basic properties and permission of application registrations'

request_body.displayName = 'ExampleCustomRole'

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission()
rolePermissionsUnifiedRolePermission1.AllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', 'Microsoft.CloudPC/CloudPCs/Reprovision', ])


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
request_body.rolepermissions(rolePermissionsArray)





result = await client.roleManagement.cloudPC.roleDefinitions_by_id('unifiedRoleDefinition-id').patch(request_body = request_body)


```