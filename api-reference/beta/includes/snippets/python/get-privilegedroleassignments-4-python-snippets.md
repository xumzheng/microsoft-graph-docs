---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PrivilegedRoleAssignmentsRequestBuilder.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters(
				filter = "isElevated eq true and expirationDateTime ne null or isElevated eq false",
)

request_configuration = PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.privilegedRoleAssignments.get(request_configuration = request_configuration)


```