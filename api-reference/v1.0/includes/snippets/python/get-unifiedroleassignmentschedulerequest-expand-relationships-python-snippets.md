---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleAssignmentScheduleRequestRequestBuilderGetRequestConfiguration(
request_config = UnifiedRoleAssignmentScheduleRequestRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["principalId","action","roleDefinitionId"]
params['expand'] = ["roleDefinition","activatedUsing","principal","targetSchedule"]
)


result = await client.roleManagement.directory.roleAssignmentScheduleRequests_by_id('unifiedRoleAssignmentScheduleRequest-id').get(request_config, headers=request_config)


```