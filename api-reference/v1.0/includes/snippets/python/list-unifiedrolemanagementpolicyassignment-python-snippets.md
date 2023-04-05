---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration(
query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "scopeId eq '/' and scopeType eq 'Directory'"

)


result = await client.policies.roleManagementPolicyAssignments.get(request_config)


```