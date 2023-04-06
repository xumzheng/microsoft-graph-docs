---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MeRequestBuilderGetRequestConfiguration(
request_config = MeRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["manager($levels=max;$select=id,displayName)"]
params['select'] = ["id","displayName"]
)
headers['ConsistencyLevel'] = "eventual"


result = await client.me.get(request_config, headers=request_config)


```