---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UnifiedRoleDefinition();
requestBody.setDescription('An example custom role');

requestBody.setDisplayName('ExampleCustomRole');

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission();
rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['Microsoft.CloudPC/CloudPCs/Read', ]);


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
requestBody.setRolePermissions(rolePermissionsArray);


additionalData = [
'condition' => 'null', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.roleManagement().cloudPC().roleDefinitions().post(requestBody);


```