---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthorizationPolicy();
defaultUserRolePermissions = DefaultUserRolePermissions();
defaultUserRolePermissions.setAllowedToCreateApps(false);


requestBody.setDefaultUserRolePermissions($defaultUserRolePermissions);


requestResult = graphServiceClient.policies().authorizationPolicyById('authorizationPolicy-id').patch(requestBody);


```