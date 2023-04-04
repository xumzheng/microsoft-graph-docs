---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = NamedLocationsRequestBuilderGetRequestConfiguration();

query_params = NamedLocationsRequestBuilderGetQueryParameters();
query_params.filter = "createdDateTime ge 2019-09-01T00:00:00Z";

request_config.queryParameters = query_params;


result = await client.identity.conditionalAccess.namedLocations.get(request_config);


```