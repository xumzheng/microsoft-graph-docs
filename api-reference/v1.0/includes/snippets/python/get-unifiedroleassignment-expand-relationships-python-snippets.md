---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UnifiedRoleAssignmentRequestBuilder.UnifiedRoleAssignmentRequestBuilderGetQueryParameters(
		expand = ["roleDefinition"],
)

request_configuration = UnifiedRoleAssignmentRequestBuilder.UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.roleManagement.directory.roleAssignments_by_id('unifiedRoleAssignment-id').get(request_configuration = request_configuration)


```