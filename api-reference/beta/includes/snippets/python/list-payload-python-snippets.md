---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PayloadsRequestBuilderGetRequestConfiguration(
request_config = PayloadsRequestBuilderGetRequestConfiguration(query_params=query_params = PayloadsRequestBuilderGetQueryParameters()
query_params.filter = "source eq 'Tenant'"

)
query_params = PayloadsRequestBuilderGetQueryParameters()
query_params.filter = "source eq 'Tenant'"

)


result = await client.security.attackSimulation.payloads.get(request_config, headers=request_config)


```