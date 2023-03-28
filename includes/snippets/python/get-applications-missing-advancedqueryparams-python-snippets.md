---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ApplicationsRequestBuilderGetRequestConfiguration();

$queryParameters = new ApplicationsRequestBuilderGetQueryParameters();
$queryParameters.search = "\"displayName:Browser\"";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.applications().get($requestConfiguration);


```