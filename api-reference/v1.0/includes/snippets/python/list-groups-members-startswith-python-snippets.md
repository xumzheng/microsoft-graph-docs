---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MembersRequestBuilderGetRequestConfiguration(
request_config = MembersRequestBuilderGetRequestConfiguration(query_params=params['count'] = true
params['filter'] = "startswith(displayName,%20'a')"
)
headers['ConsistencyLevel'] = "eventual"


result = await client.groups_by_id('group-id').members.get(request_config, headers=request_config)


```