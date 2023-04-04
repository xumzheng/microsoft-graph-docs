---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnifiedRoleDefinition()
request_body.setDescription('Update basic properties and permission of application registrations')

request_body.setDisplayName('ExampleCustomRole')

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission()
rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', 'Microsoft.CloudPC/CloudPCs/Reprovision', ])


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
request_body.setRolePermissions(rolePermissionsArray)




result = await client.roleManagement.cloudPC.roleDefinitionsById('unifiedRoleDefinition-id').patch(request_body)


```