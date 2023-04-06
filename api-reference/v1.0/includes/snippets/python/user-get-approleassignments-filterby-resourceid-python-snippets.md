---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AppRoleAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = AppRoleAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = AppRoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "resourceId eq 8e881353-1735-45af-af21-ee1344582a4d"

)
query_params = AppRoleAssignmentsRequestBuilderGetQueryParameters()
query_params['filter'] = "resourceId eq 8e881353-1735-45af-af21-ee1344582a4d"

)


result = await client.users_by_id('user-id').appRoleAssignments.get(request_configuration)


```