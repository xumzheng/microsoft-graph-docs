---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MeRequestBuilderGetRequestConfiguration(
request_config = MeRequestBuilderGetRequestConfiguration(query_params=query_params = MeRequestBuilderGetQueryParameters()
query_params.expand = ["manager($levels=max;$select=id,displayName)"]
query_params.select = ["id","displayName"]

)
query_params = MeRequestBuilderGetQueryParameters()
query_params.expand = ["manager($levels=max;$select=id,displayName)"]
query_params.select = ["id","displayName"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.get(request_config, headers=request_config)


```