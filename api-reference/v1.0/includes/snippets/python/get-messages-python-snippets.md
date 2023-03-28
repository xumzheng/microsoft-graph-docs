---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters.select = ["sender","subject"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().messages().get($requestConfiguration);


```