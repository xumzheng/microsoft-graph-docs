---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
request_config = GroupsRequestBuilderGetRequestConfiguration(query_params=params['search'] = "\"displayName:OneVideo\" OR \"mail:onevideo\""
)
headers['ConsistencyLevel'] = "eventual"


result = await client.groups.get(request_config, headers=request_config)


```