---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UserProcessingResultsRequestBuilderGetRequestConfiguration();

queryParameters = UserProcessingResultsRequestBuilderGetQueryParameters();
queryParameters.select = ["id","failedTasksCount","processingStatus","totalTasksCount","totalUnprocessedTasksCount","subject"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').runsById('run-id').userProcessingResults().get(requestConfiguration);


```