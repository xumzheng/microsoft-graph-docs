---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = IncidentsRequestBuilderGetRequestConfiguration(
request_configuration = IncidentsRequestBuilderGetRequestConfiguration(query_params=query_params = IncidentsRequestBuilderGetQueryParameters()
query_params['expand'] = ["alerts"]

)
query_params = IncidentsRequestBuilderGetQueryParameters()
query_params['expand'] = ["alerts"]

)


result = await client.security.incidents.get(request_configuration)


```