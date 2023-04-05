---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleManagementPolicyAssignmentRequestBuilderGetRequestConfiguration()

query_params = UnifiedRoleManagementPolicyAssignmentRequestBuilderGetQueryParameters()
query_params.expand = ["policy($expand=rules)"]

request_config.queryParameters = query_params


result = await client.policies.roleManagementPolicyAssignmentsById('unifiedRoleManagementPolicyAssignment-id').get(request_config)


```