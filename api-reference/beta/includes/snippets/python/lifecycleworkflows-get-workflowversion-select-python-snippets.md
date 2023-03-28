---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new WorkflowVersionRequestBuilderGetRequestConfiguration();

$queryParameters = new WorkflowVersionRequestBuilderGetQueryParameters();
$queryParameters.select = ["category","displayName","versionNumber","executionConditions"];
$queryParameters.expand = ["tasks"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').versionsById('workflowVersion-versionNumber').get($requestConfiguration);


```