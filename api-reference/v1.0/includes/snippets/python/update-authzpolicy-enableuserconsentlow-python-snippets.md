---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy()
defaultUserRolePermissions = DefaultUserRolePermissions()
defaultUserRolePermissions.setPermissionGrantPoliciesAssigned(['managePermissionGrantsForSelf.microsoft-user-default-low', ])


request_body.setDefaultUserRolePermissions($defaultUserRolePermissions)

request_config = AuthorizationPolicyRequestBuilderPatchRequestConfiguration(
request_config = AuthorizationPolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.authorizationPolicy.patch(request_body, headers=)


```