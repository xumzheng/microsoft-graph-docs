---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration(
request_config = GroupRequestBuilderGetRequestConfiguration(query_params=params['count'] = true
params['orderby'] = ["deletedDateTime asc"]
params['select'] = ["id","displayName","deletedDateTime"]
)
headers['ConsistencyLevel'] = "eventual"


result = await client.directory.deletedItems.graphgroup.get(request_config, headers=request_config)


```