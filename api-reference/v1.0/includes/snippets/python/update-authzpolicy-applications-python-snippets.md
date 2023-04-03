---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthorizationPolicy();
defaultUserRolePermissions = DefaultUserRolePermissions();
defaultUserRolePermissions.setAllowedToCreateApps(false);


requestBody.setDefaultUserRolePermissions($defaultUserRolePermissions);


result = awaitclient.policies().authorizationPolicy().patch(requestBody);


```