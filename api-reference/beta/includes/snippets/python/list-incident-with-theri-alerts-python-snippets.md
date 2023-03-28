---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new IncidentsRequestBuilderGetRequestConfiguration();

$queryParameters = new IncidentsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["alerts"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.security().incidents().get($requestConfiguration);


```