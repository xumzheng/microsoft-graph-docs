---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UserProcessingResultsRequestBuilderGetRequestConfiguration(
request_configuration = UserProcessingResultsRequestBuilderGetRequestConfiguration(query_params=query_params = UserProcessingResultsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"]

)
query_params = UserProcessingResultsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs_by_id('run-id').userProcessingResults.get(request_configuration)


```