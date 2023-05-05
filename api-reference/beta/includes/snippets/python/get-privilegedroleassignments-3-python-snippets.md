---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PrivilegedRoleAssignmentsRequestBuilder.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters(
		filter = "isElevated eq true and expirationDateTime eq null",
)

request_configuration = PrivilegedRoleAssignmentsRequestBuilder.PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.privileged_role_assignments.get(request_configuration = request_configuration)


```