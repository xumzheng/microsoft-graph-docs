---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new DefinitionsRequestBuilderGetQueryParameters();
$queryParameters->top = 100;
$queryParameters->skip = 0;

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->accessReviews()->definitions()->get($requestConfiguration);


```