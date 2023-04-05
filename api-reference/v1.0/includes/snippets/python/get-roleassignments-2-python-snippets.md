---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration()

query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = " principalId eq '5bde3e51-d13b-4db1-9948-fe4b109d11a7'"

request_config.queryParameters = query_params


result = await client.roleManagement.directory.roleAssignments.get(request_config)


```