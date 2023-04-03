---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = B2xUserFlowsRequestBuilderGetRequestConfiguration();

query_params = B2xUserFlowsRequestBuilderGetQueryParameters();
query_params.expand = ["identityProviders"];

request_config.queryParameters = query_params;


result = await client.identity().b2xUserFlows().get(request_config);


```