---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters->filter = "isof or isof";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->directoryObjects()->delta()->get($requestConfiguration);


```