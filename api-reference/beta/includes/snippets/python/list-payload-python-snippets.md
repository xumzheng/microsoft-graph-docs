---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PayloadsRequestBuilder.PayloadsRequestBuilderGetQueryParameters(
		filter = "source eq 'Tenant'",
)

request_configuration = PayloadsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.security.attackSimulation.payloads.get(request_configuration = request_configuration)


```