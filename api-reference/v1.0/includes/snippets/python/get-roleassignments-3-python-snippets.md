---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration()

query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'"
query_params.expand = ["principal"]

request_config.queryParameters = query_params


result = await client.roleManagement_entitlementManagement_roleAssignments.get(request_config)


```