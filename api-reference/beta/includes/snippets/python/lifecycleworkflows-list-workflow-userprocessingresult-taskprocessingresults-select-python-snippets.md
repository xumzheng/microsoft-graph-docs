---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TaskProcessingResultsRequestBuilderGetRequestConfiguration();

query_params = TaskProcessingResultsRequestBuilderGetQueryParameters();
query_params.select = ["id","failureReason","processingStatus","subject","task"];

request_config.queryParameters = query_params;


result = awaitclient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').runsById('run-id').userProcessingResultsById('userProcessingResult-id').taskProcessingResults().get(request_config);


```