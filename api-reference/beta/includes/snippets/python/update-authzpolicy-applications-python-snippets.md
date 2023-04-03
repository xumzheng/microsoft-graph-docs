---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthorizationPolicy();
defaultUserRolePermissions = DefaultUserRolePermissions();
defaultUserRolePermissions.setAllowedToCreateApps(false);


requestBody.setDefaultUserRolePermissions($defaultUserRolePermissions);


result = await client.policies().authorizationPolicyById('authorizationPolicy-id').patch(requestBody);


```