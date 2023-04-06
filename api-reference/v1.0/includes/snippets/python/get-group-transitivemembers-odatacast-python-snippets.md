---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration(
request_config = GroupRequestBuilderGetRequestConfiguration(query_params=query_params = GroupRequestBuilderGetQueryParameters()
query_params.count = true

)
query_params = GroupRequestBuilderGetQueryParameters()
query_params.count = true

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups_by_id('group-id').transitiveMembers.graphgroup.get(request_config, headers=request_config)


```