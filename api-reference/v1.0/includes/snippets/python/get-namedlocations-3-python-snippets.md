---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new NamedLocationsRequestBuilderGetRequestConfiguration();

$queryParameters = new NamedLocationsRequestBuilderGetQueryParameters();
$queryParameters.filter = "createdDateTime ge 2019-09-01T00:00:00Z";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identity().conditionalAccess().namedLocations().get($requestConfiguration);


```