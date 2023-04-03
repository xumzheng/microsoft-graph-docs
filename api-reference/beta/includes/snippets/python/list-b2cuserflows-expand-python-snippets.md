---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = B2cUserFlowsRequestBuilderGetRequestConfiguration();

query_params = B2cUserFlowsRequestBuilderGetQueryParameters();
query_params.expand = ["identityProviders"];

request_config.queryParameters = query_params;


result = awaitclient.identity().b2cUserFlows().get(request_config);


```