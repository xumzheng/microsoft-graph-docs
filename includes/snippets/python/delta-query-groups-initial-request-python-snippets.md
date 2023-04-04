---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = DeltaRequestBuilderGetRequestConfiguration()

query_params = DeltaRequestBuilderGetQueryParameters()
query_params.select = ["displayName","description","members"]

request_config.queryParameters = query_params


result = await client.groups.delta.get(request_config)


```