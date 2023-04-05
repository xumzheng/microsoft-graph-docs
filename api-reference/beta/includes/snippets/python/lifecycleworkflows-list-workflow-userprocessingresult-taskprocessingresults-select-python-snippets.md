---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TaskProcessingResultsRequestBuilderGetRequestConfiguration()

query_params = TaskProcessingResultsRequestBuilderGetQueryParameters()
query_params.select = ["id","failureReason","processingStatus","subject","task"]

request_config.queryParameters = query_params


result = await client.identityGovernance_lifecycleWorkflows_workflowsby_id('workflow-id')_runsby_id('run-id')_userProcessingResultsby_id('userProcessingResult-id')_taskProcessingResults.get(request_config)


```