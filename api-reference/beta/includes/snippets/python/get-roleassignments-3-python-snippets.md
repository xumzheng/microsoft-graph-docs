---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration(
request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'"
params['expand'] = ["principal"]
)


result = await client.roleManagement.entitlementManagement.roleAssignments.get(request_config, headers=request_config)


```