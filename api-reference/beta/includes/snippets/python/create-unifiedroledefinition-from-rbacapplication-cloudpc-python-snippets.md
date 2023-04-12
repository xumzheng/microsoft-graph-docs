---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleDefinition()
request_body.description = 'An example custom role'

request_body.displayName = 'ExampleCustomRole'

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission()
rolePermissionsUnifiedRolePermission1.AllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', ])


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
request_body.rolepermissions(rolePermissionsArray)


additionalData = [
'condition' => 'null', 
];
request_body.additionaldata(additionalData)





result = await client.roleManagement.cloudPC.roleDefinitions.post(request_body = request_body)


```