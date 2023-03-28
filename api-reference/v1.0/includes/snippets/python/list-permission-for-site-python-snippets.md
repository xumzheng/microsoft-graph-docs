---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new SitesRequestBuilderGetRequestConfiguration();

$queryParameters = new SitesRequestBuilderGetQueryParameters();
$queryParameters->search = "{query}";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->sites()->get($requestConfiguration);


```