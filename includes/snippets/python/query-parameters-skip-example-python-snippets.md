---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new EventsRequestBuilderGetRequestConfiguration();

$queryParameters = new EventsRequestBuilderGetQueryParameters();
$queryParameters.orderby = ["createdDateTime"];
$queryParameters.skip = 20;

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().events().get($requestConfiguration);


```