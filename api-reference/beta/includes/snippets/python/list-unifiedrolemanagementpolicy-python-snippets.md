---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleManagementPoliciesRequestBuilderGetRequestConfiguration()

query_params = RoleManagementPoliciesRequestBuilderGetQueryParameters()
query_params.filter = "scopeId eq '/' and scopeType eq 'DirectoryRole'"

request_config.queryParameters = query_params


result = await client.policies.roleManagementPolicies.get(request_config)


```