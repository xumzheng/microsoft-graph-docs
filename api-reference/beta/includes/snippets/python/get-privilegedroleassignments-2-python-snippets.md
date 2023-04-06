---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "isElevated eq true"

)
query_params = PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "isElevated eq true"

)


result = await client.privilegedRoleAssignments.get(request_configuration)


```