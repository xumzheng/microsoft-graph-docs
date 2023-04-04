---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnifiedRoleDefinition();
request_body.setDescription('Update basic properties of application registrations');

request_body.setDisplayName('Application Registration Support Administrator');

rolePermissionsUnifiedRolePermission1 = UnifiedRolePermission();
rolePermissionsUnifiedRolePermission1.setAllowedResourceActions(['microsoft.directory/applications/basic/read', ]);


rolePermissionsArray []= rolePermissionsUnifiedRolePermission1;
request_body.setRolePermissions(rolePermissionsArray);




result = await client.roleManagement.directory.roleDefinitionsById('unifiedRoleDefinition-id').patch(request_body);


```