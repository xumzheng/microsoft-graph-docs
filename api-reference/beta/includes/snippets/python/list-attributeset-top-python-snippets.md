---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AttributeSetsRequestBuilderGetRequestConfiguration();

$queryParameters = new AttributeSetsRequestBuilderGetQueryParameters();
$queryParameters->top = 10;

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->directory()->attributeSets()->get($requestConfiguration);


```