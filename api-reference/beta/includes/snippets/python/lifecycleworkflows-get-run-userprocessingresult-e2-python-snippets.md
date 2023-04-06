---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserProcessingResultRequestBuilderGetRequestConfiguration(
request_config = UserProcessingResultRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"]
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs_by_id('run-id').userProcessingResults_by_id('userProcessingResult-id').get(request_config, headers=request_config)


```