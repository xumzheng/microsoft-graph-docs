---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "scopeId eq '/' and scopeType eq 'Directory'"

)
query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "scopeId eq '/' and scopeType eq 'Directory'"

)


result = await client.policies.roleManagementPolicyAssignments.get(request_configuration)


```