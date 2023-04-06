---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DevicesRequestBuilderGetRequestConfiguration(
request_config = DevicesRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "startswith(displayName,%20'a')"
params['count'] = true
params['top'] = 1
params['orderby'] = ["displayName"]
)
headers['ConsistencyLevel'] = "eventual"


result = await client.devices.get(request_config, headers=request_config)


```