---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new EventsRequestBuilderGetRequestConfiguration();

$queryParameters = new EventsRequestBuilderGetQueryParameters();
$queryParameters.filter = "startsWith(subject,'All')";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().calendar().events().get($requestConfiguration);


```