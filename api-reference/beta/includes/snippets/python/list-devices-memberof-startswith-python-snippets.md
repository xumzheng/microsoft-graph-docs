---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration(
request_config = GroupRequestBuilderGetRequestConfiguration(query_params=params['count'] = true
params['orderby'] = ["displayName"]
params['filter'] = "startswith(displayName,%20'A')"
)
headers['ConsistencyLevel'] = "eventual"


result = await client.devices_by_id('device-id').memberOf.graphgroup.get(request_config, headers=request_config)


```