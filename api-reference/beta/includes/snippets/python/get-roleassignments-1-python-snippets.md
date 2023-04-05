---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration()

query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'"
query_params.expand = ["principal"]

request_config.queryParameters = query_params


result = await client.roleManagement.directory.roleAssignments.get(request_config)


```