---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = NamedLocationsRequestBuilderGetRequestConfiguration(
request_config = NamedLocationsRequestBuilderGetRequestConfiguration(query_params=query_params = NamedLocationsRequestBuilderGetQueryParameters()
query_params.filter = "microsoft.graph.countryNamedLocation/countriesAndRegions/any"

)
query_params = NamedLocationsRequestBuilderGetQueryParameters()
query_params.filter = "microsoft.graph.countryNamedLocation/countriesAndRegions/any"

)


result = await client.identity.conditionalAccess.namedLocations.get(request_config, headers=request_config)


```