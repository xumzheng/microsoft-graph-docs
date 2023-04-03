---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TaskProcessingResultsRequestBuilderGetRequestConfiguration();

queryParameters = TaskProcessingResultsRequestBuilderGetQueryParameters();
queryParameters.select = ["id","failureReason","processingStatus","subject","task"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').taskReportsById('taskReport-id').taskProcessingResults().get(requestConfiguration);


```