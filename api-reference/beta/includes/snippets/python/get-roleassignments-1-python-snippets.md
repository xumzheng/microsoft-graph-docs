---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RoleAssignmentsRequestBuilder.RoleAssignmentsRequestBuilderGetQueryParameters(
				filter = "roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'",
				expand = ["principal"],
)

request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.roleManagement.directory.roleAssignments.get(request_configuration = request_configuration)


```