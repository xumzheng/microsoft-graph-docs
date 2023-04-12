---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TaskProcessingResultsRequestBuilder.TaskProcessingResultsRequestBuilderGetQueryParameters(
		select = ["id","failureReason","processingStatus","subject"],
)

request_configuration = TaskProcessingResultsRequestBuilder.TaskProcessingResultsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').runs_by_id('run-id').taskProcessingResults.get(request_configuration = request_configuration)


```