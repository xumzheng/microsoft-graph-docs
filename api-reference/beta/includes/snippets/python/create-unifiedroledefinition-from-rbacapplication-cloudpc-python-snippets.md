---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnifiedRoleDefinition();
$requestBody.setDescription('An example custom role');

$requestBody.setDisplayName('ExampleCustomRole');

$rolePermissionsUnifiedRolePermission1 = new UnifiedRolePermission();
$rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', ]);


$rolePermissionsArray []= $rolePermissionsUnifiedRolePermission1;
$requestBody.setRolePermissions($rolePermissionsArray);


$additionalData = [
'condition' => 'null', 
];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.roleManagement().cloudPC().roleDefinitions().post($requestBody);


```