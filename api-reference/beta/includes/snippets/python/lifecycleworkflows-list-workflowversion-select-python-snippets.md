---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new VersionsRequestBuilderGetRequestConfiguration();

$queryParameters = new VersionsRequestBuilderGetQueryParameters();
$queryParameters.select = ["category","displayName","versionNumber"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').versions().get($requestConfiguration);


```