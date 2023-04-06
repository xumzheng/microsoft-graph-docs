---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'"
query_params['expand'] = ["policy($expand=rules)"]

)
query_params = RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'"
query_params['expand'] = ["policy($expand=rules)"]

)


result = await client.policies.roleManagementPolicyAssignments.get(request_configuration)


```