---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RoleAssignmentScheduleRequestsRequestBuilderGetRequestConfiguration(
request_configuration = RoleAssignmentScheduleRequestsRequestBuilderGetRequestConfiguration(query_params=query_params = RoleAssignmentScheduleRequestsRequestBuilderGetQueryParameters()
query_params['select'] = ["principalId","action","roleDefinitionId"]
query_params['expand'] = ["roleDefinition","activatedUsing","principal","targetSchedule"]

)
query_params = RoleAssignmentScheduleRequestsRequestBuilderGetQueryParameters()
query_params['select'] = ["principalId","action","roleDefinitionId"]
query_params['expand'] = ["roleDefinition","activatedUsing","principal","targetSchedule"]

)


result = await client.roleManagement.directory.roleAssignmentScheduleRequests.get(request_configuration)


```