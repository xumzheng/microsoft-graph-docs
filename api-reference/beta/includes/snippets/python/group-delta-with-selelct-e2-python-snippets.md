---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration(
request_config = DeltaRequestBuilderGetRequestConfiguration(query_params=query_params = DeltaRequestBuilderGetQueryParameters()
query_params.select = ["displayName","description","mailNickname"]

)
query_params = DeltaRequestBuilderGetQueryParameters()
query_params.select = ["displayName","description","mailNickname"]

)


result = await client.groups.delta.get(request_config, headers=request_config)


```