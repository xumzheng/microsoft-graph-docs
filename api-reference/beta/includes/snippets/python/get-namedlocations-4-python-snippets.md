---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new NamedLocationsRequestBuilderGetRequestConfiguration();

$queryParameters = new NamedLocationsRequestBuilderGetQueryParameters();
$queryParameters.filter = "microsoft.graph.countryNamedLocation/countriesAndRegions/any";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identity().conditionalAccess().namedLocations().get($requestConfiguration);


```