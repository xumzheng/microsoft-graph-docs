---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters->select = ["displayName","givenName","surname"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->users()->delta()->get($requestConfiguration);


```