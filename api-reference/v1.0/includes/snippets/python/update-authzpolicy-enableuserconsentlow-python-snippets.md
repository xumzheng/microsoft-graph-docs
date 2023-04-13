---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy()
default_user_role_permissions = DefaultUserRolePermissions()
defaultUserRolePermissions.PermissionGrantPoliciesAssigned(['managePermissionGrantsForSelf.microsoft-user-default-low', ])


request_body.default_user_role_permissions = defaultUserRolePermissions



result = await client.policies.authorizationPolicy.patch(request_body = request_body)


```