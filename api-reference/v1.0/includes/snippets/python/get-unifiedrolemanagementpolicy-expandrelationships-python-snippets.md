---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = UnifiedRoleManagementPolicyRequestBuilderGetRequestConfiguration();

query_params = UnifiedRoleManagementPolicyRequestBuilderGetQueryParameters();
query_params.expand = ["effectiveRules","rules"];

request_config.queryParameters = query_params;


result = awaitclient.policies().roleManagementPoliciesById('unifiedRoleManagementPolicy-id').get(request_config);


```