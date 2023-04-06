---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleManagementPoliciesRequestBuilderGetRequestConfiguration(
request_config = RoleManagementPoliciesRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "scopeId eq '/' and scopeType eq 'Directory'"
params['expand'] = ["rules"]
)


result = await client.policies.roleManagementPolicies.get(request_config, headers=request_config)


```