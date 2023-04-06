---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration(
request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'"

)
query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'"

)


result = await client.roleManagement.cloudPC.roleAssignments.get(request_config, headers=request_config)


```