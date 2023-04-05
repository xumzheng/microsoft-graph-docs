---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleManagementPolicyRequestBuilderGetRequestConfiguration()

query_params = UnifiedRoleManagementPolicyRequestBuilderGetQueryParameters()
query_params.expand = ["effectiveRules","rules"]

request_config.queryParameters = query_params


result = await client.policies.roleManagementPolicies._by_id('unifiedRoleManagementPolicy-id').get(request_config)


```