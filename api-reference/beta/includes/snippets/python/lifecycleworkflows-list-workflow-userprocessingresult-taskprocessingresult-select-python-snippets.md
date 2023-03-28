---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TaskProcessingResultsRequestBuilderGetRequestConfiguration();

$queryParameters = new TaskProcessingResultsRequestBuilderGetQueryParameters();
$queryParameters.select = ["id","processingStatus","failureReason","subject","task"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').userProcessingResultsById('userProcessingResult-id').taskProcessingResults().get($requestConfiguration);


```