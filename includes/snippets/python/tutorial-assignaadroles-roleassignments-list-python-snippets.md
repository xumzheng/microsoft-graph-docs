---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'"

)
query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'"

)


result = await client.roleManagement.directory.roleAssignments.get(request_configuration)


```