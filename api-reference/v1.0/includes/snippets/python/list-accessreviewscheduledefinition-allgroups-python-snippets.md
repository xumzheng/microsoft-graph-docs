---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new DefinitionsRequestBuilderGetQueryParameters();
$queryParameters->filter = "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityGovernance()->accessReviews()->definitions()->get($requestConfiguration);


```