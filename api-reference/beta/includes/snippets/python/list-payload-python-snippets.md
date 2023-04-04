---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = PayloadsRequestBuilderGetRequestConfiguration();

query_params = PayloadsRequestBuilderGetQueryParameters();
query_params.filter = "source eq 'Tenant'";

request_config.queryParameters = query_params;


result = await client.security.attackSimulation.payloads.get(request_config);


```