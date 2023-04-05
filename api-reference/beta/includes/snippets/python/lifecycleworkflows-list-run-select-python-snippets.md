---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RunsRequestBuilderGetRequestConfiguration(
query_params = RunsRequestBuilderGetQueryParameters()
query_params.select = ["id","failedTasksCount","failedUsersCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","totalUsersCount","id"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs.get(request_config)


```