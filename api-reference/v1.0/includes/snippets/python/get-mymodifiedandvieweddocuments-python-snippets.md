---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new UsedRequestBuilderGetRequestConfiguration();

$queryParameters = new UsedRequestBuilderGetQueryParameters();
$queryParameters.orderby = ["LastUsed/LastAccessedDateTime desc"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().insights().used().get($requestConfiguration);


```