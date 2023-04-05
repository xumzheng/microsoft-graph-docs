---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TaskProcessingResultsRequestBuilderGetRequestConfiguration()

query_params = TaskProcessingResultsRequestBuilderGetQueryParameters()
query_params.select = ["id","processingStatus","failureReason","subject","task"]

request_config.queryParameters = query_params


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').userProcessingResults_by_id('userProcessingResult-id').taskProcessingResults.get(request_config)


```