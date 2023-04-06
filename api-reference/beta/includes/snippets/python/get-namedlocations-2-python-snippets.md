---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = NamedLocationsRequestBuilderGetRequestConfiguration(
request_configuration = NamedLocationsRequestBuilderGetRequestConfiguration(query_params=query_params = NamedLocationsRequestBuilderGetQueryParameters()
query_params['filter'] = "isof('microsoft.graph.ipNamedLocation')"

)
query_params = NamedLocationsRequestBuilderGetQueryParameters()
query_params['filter'] = "isof('microsoft.graph.ipNamedLocation')"

)


result = await client.identity.conditionalAccess.namedLocations.get(request_configuration)


```