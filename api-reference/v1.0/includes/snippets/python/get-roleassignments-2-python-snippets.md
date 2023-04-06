---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = RoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = " principalId eq '5bde3e51-d13b-4db1-9948-fe4b109d11a7'"

)
query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = " principalId eq '5bde3e51-d13b-4db1-9948-fe4b109d11a7'"

)


result = await client.roleManagement.directory.roleAssignments.get(request_configuration)


```