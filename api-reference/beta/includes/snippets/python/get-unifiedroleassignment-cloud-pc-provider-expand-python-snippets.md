---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UnifiedRoleAssignmentMultipleRequestBuilder.UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters(
				expand = ["roleDefinition"],
)

request_configuration = UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.roleManagement.cloudPC.roleAssignments_by_id('unifiedRoleAssignmentMultiple-id').get(request_configuration = request_configuration)


```