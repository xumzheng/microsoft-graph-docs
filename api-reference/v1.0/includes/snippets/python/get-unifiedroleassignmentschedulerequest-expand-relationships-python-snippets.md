---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UnifiedRoleAssignmentScheduleRequestRequestBuilderGetRequestConfiguration()

query_params = UnifiedRoleAssignmentScheduleRequestRequestBuilderGetQueryParameters()
query_params.select = ["principalId","action","roleDefinitionId"]
query_params.expand = ["roleDefinition","activatedUsing","principal","targetSchedule"]

request_config.queryParameters = query_params


result = await client.roleManagement.directory.roleAssignmentScheduleRequestsby_id('unifiedRoleAssignmentScheduleRequest-id').get(request_config)


```