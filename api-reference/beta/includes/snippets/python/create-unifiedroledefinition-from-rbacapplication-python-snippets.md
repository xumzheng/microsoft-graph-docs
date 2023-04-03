---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedRoleDefinition();
requestBody.setDescription('Update basic properties of application registrations');

requestBody.setDisplayName('Application Registration Support Administrator');

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission();
rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['microsoft.directory/applications/basic/read', ]);


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
requestBody.setRolePermissions(rolePermissionsArray);


requestBody.setIsEnabled(true);



result = await client.roleManagement().directory().roleDefinitions().post(requestBody);


```