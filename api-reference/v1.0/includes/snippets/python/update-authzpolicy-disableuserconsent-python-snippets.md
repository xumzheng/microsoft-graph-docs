---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Authorization_policy()
default_user_role_permissions = Default_user_role_permissions()
default_user_role_permissions.PermissionGrantPoliciesAssigned([])


request_body.default_user_role_permissions = default_user_role_permissions



result = await client.policies.authorization_policy.patch(request_body = request_body)


```