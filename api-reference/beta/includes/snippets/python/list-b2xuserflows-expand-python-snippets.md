---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = B2xUserFlowsRequestBuilderGetRequestConfiguration(
request_configuration = B2xUserFlowsRequestBuilderGetRequestConfiguration(query_params=query_params = B2xUserFlowsRequestBuilderGetQueryParameters()
query_params['expand'] = ["identityProviders"]

)
query_params = B2xUserFlowsRequestBuilderGetQueryParameters()
query_params['expand'] = ["identityProviders"]

)


result = await client.identity.b2xUserFlows.get(request_configuration)


```