---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RunsRequestBuilder.RunsRequestBuilderGetQueryParameters(
		select = ["id","failedTasksCount","failedUsersCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","totalUsersCount","id"],
)

request_configuration = RunsRequestBuilder.RunsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs.get(request_configuration = request_configuration)


```