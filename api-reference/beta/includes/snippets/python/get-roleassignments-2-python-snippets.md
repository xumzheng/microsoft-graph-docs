---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RoleAssignmentsRequestBuilder.RoleAssignmentsRequestBuilderGetQueryParameters(
				filter = " principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'",
)

request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.roleManagement.directory.roleAssignments.get(request_configuration = request_configuration)


```