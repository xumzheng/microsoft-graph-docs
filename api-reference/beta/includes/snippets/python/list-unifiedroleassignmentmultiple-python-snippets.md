---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RoleAssignmentsRequestBuilderGetRequestConfiguration()

query_params = RoleAssignmentsRequestBuilderGetQueryParameters()
query_params.filter = "principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'"

request_config.queryParameters = query_params


result = await client.roleManagement.deviceManagement.roleAssignments.get(request_config)


```