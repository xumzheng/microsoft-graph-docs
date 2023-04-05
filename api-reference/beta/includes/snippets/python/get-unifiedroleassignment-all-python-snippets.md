---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration(
query_params = TransitiveRoleAssignmentsRequestBuilderGetQueryParameters()
query_params.count = true
query_params.filter = "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'"

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.roleManagement.directory.transitiveRoleAssignments.get(request_config)


```