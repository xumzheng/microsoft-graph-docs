---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserProcessingResultsRequestBuilderGetRequestConfiguration()

query_params = UserProcessingResultsRequestBuilderGetQueryParameters()
query_params.select = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"]

request_config.queryParameters = query_params


result = await client.identityGovernance.lifecycleWorkflows.workflows._by_id('workflow-id').runs._by_id('run-id').userProcessingResults.get(request_config)


```