---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RunRequestBuilderGetRequestConfiguration(
request_configuration = RunRequestBuilderGetRequestConfiguration(query_params=query_params = RunRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedTasksCount","failedUsersCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","totalUsersCount"]

)
query_params = RunRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedTasksCount","failedUsersCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","totalUsersCount"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs_by_id('run-id').get(request_configuration)


```