---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnifiedRoleDefinition();
$requestBody.setDescription('Update basic properties and permission of application registrations');

$requestBody.setDisplayName('ExampleCustomRole');

$rolePermissionsUnifiedRolePermission1 = new UnifiedRolePermission();
$rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', 'Microsoft.CloudPC/CloudPCs/Reprovision', ]);


$rolePermissionsArray []= $rolePermissionsUnifiedRolePermission1;
$requestBody.setRolePermissions($rolePermissionsArray);




$requestResult = $graphServiceClient.roleManagement().cloudPC().roleDefinitionsById('unifiedRoleDefinition-id').patch($requestBody);


```