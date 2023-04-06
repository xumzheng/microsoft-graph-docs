---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = B2cUserFlowsRequestBuilderGetRequestConfiguration(
request_configuration = B2cUserFlowsRequestBuilderGetRequestConfiguration(query_params=query_params = B2cUserFlowsRequestBuilderGetQueryParameters()
query_params['expand'] = ["identityProviders"]

)
query_params = B2cUserFlowsRequestBuilderGetQueryParameters()
query_params['expand'] = ["identityProviders"]

)


result = await client.identity.b2cUserFlows.get(request_configuration)


```