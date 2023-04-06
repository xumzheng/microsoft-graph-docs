---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TaskProcessingResultsRequestBuilderGetRequestConfiguration(
request_configuration = TaskProcessingResultsRequestBuilderGetRequestConfiguration(query_params=query_params = TaskProcessingResultsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","processingStatus","failureReason","subject","task"]

)
query_params = TaskProcessingResultsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","processingStatus","failureReason","subject","task"]

)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').userProcessingResults_by_id('userProcessingResult-id').taskProcessingResults.get(request_configuration)


```