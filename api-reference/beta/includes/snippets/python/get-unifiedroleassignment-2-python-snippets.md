---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration(
request_config = UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration(query_params=query_params = UnifiedRoleAssignmentRequestBuilderGetQueryParameters()
query_params.expand = ["roleDefinition"]

)
query_params = UnifiedRoleAssignmentRequestBuilderGetQueryParameters()
query_params.expand = ["roleDefinition"]

)


result = await client.roleManagement.directory.roleAssignments_by_id('unifiedRoleAssignment-id').get(request_config, headers=request_config)


```