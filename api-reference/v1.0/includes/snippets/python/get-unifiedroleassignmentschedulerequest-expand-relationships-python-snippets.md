---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UnifiedRoleAssignmentScheduleRequestRequestBuilder.UnifiedRoleAssignmentScheduleRequestRequestBuilderGetQueryParameters(
		select = ["principalId","action","roleDefinitionId"],
		expand = ["roleDefinition","activatedUsing","principal","targetSchedule"],
)

request_configuration = UnifiedRoleAssignmentScheduleRequestRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.roleManagement.directory.roleAssignmentScheduleRequests_by_id('unifiedRoleAssignmentScheduleRequest-id').get(request_configuration = request_configuration)


```