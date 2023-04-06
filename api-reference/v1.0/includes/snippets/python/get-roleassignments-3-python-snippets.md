---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'"
query_params['expand'] = ["principal"]

)
query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'"
query_params['expand'] = ["principal"]

)


result = await client.roleManagement.entitlementManagement.roleAssignments.get(request_configuration)


```