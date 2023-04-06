---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = TransitiveRoleAssignmentsRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['filter'] = "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'"

)
query_params = TransitiveRoleAssignmentsRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['filter'] = "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.roleManagement.directory.transitiveRoleAssignments.get(request_configuration)


```