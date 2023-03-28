---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TaskDefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new TaskDefinitionsRequestBuilderGetQueryParameters();
$queryParameters->filter = "category has 'joiner'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->lifecycleWorkflows()->taskDefinitions()->get($requestConfiguration);


```