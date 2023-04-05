---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = IncidentsRequestBuilderGetRequestConfiguration()

query_params = IncidentsRequestBuilderGetQueryParameters()
query_params.expand = ["alerts"]

request_config.queryParameters = query_params


result = await client.security_incidents.get(request_config)


```