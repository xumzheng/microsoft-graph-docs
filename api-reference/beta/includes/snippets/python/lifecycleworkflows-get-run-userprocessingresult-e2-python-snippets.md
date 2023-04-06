---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UserProcessingResultRequestBuilderGetRequestConfiguration(
request_configuration = UserProcessingResultRequestBuilderGetRequestConfiguration(query_params=query_params = UserProcessingResultRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"]

)
query_params = UserProcessingResultRequestBuilderGetQueryParameters()
query_params['select'] = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs_by_id('run-id').userProcessingResults_by_id('userProcessingResult-id').get(request_configuration)


```