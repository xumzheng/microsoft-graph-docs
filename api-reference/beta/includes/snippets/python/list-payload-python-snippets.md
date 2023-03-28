---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PayloadsRequestBuilderGetRequestConfiguration();

$queryParameters = new PayloadsRequestBuilderGetQueryParameters();
$queryParameters.filter = "source eq 'Tenant'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.security().attackSimulation().payloads().get($requestConfiguration);


```