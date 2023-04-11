---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy()
defaultUserRolePermissions = DefaultUserRolePermissions()
defaultUserRolePermissions.allowedToCreateApps = false


request_body.defaultUserRolePermissions = defaultUserRolePermissions



result = await client.policies.authorizationPolicy.patch(request_body = request_body)


```