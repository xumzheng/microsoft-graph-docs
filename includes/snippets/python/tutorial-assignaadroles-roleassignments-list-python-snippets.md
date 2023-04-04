---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration()

query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'"

request_config.queryParameters = query_params


result = await client.roleManagement.directory.roleAssignments.get(request_config)


```