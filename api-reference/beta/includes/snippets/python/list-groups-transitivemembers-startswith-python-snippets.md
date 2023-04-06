---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserRequestBuilderGetRequestConfiguration(
request_config = UserRequestBuilderGetRequestConfiguration(query_params=params['count'] = true
params['orderby'] = ["displayName"]
params['filter'] = "startswith(displayName,%20'a')"
)
headers['ConsistencyLevel'] = "eventual"


result = await client.groups_by_id('group-id').transitiveMembers.graphuser.get(request_config, headers=request_config)


```