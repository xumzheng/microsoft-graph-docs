---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UnifiedRoleManagementPolicyAssignmentRequestBuilderGetRequestConfiguration(
request_configuration = UnifiedRoleManagementPolicyAssignmentRequestBuilderGetRequestConfiguration(query_params=query_params = UnifiedRoleManagementPolicyAssignmentRequestBuilderGetQueryParameters()
query_params['expand'] = ["policy($expand=rules)"]

)
query_params = UnifiedRoleManagementPolicyAssignmentRequestBuilderGetQueryParameters()
query_params['expand'] = ["policy($expand=rules)"]

)


result = await client.policies.roleManagementPolicyAssignments_by_id('unifiedRoleManagementPolicyAssignment-id').get(request_configuration)


```