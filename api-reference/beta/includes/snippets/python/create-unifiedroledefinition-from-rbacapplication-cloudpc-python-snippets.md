---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleDefinition()
request_body.setDescription('An example custom role')

request_body.setDisplayName('ExampleCustomRole')

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission()
rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', ])


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
request_body.setRolePermissions(rolePermissionsArray)


additionalData = [
'condition' => 'null', 
];
request_body.setAdditionalData(additionalData)




result = await client.roleManagement.cloudPC.roleDefinitions.post(request_body)


```