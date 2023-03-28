---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new WorkflowRequestBuilderGetRequestConfiguration();

$queryParameters = new WorkflowRequestBuilderGetQueryParameters();
$queryParameters.select = ["id","category","displayName","description","version","executionConditions"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().lifecycleWorkflows().deletedItems().workflowsById('workflow-id').get($requestConfiguration);


```