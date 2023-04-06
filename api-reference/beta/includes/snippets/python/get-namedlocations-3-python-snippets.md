---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = NamedLocationsRequestBuilderGetRequestConfiguration(
request_configuration = NamedLocationsRequestBuilderGetRequestConfiguration(query_params=query_params = NamedLocationsRequestBuilderGetQueryParameters()
query_params['filter'] = "createdDateTime ge 2019-09-01T00:00:00Z"

)
query_params = NamedLocationsRequestBuilderGetQueryParameters()
query_params['filter'] = "createdDateTime ge 2019-09-01T00:00:00Z"

)


result = await client.identity.conditionalAccess.namedLocations.get(request_configuration)


```