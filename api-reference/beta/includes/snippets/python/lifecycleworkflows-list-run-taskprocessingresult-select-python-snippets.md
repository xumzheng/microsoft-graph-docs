---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TaskProcessingResultsRequestBuilderGetRequestConfiguration(
request_config = TaskProcessingResultsRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","failureReason","processingStatus","subject"]
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs_by_id('run-id').taskProcessingResults.get(request_config, headers=request_config)


```