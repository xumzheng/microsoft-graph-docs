---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TaskProcessingResultsRequestBuilderGetRequestConfiguration()

query_params = TaskProcessingResultsRequestBuilderGetQueryParameters()
query_params.select = ["id","failureReason","processingStatus","subject"]

request_config.queryParameters = query_params


result = await client.identityGovernance.lifecycleWorkflows.workflowsById('workflow-id').runsById('run-id').taskProcessingResults.get(request_config)


```