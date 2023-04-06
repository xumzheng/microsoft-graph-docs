---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
request_config = GroupsRequestBuilderGetRequestConfiguration(query_params=query_params = GroupsRequestBuilderGetQueryParameters()
query_params.search = "\"displayName:Video\" OR \"description:prod\""
query_params.orderby = ["displayName"]
query_params.count = true

)
query_params = GroupsRequestBuilderGetQueryParameters()
query_params.search = "\"displayName:Video\" OR \"description:prod\""
query_params.orderby = ["displayName"]
query_params.count = true

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups.get(request_config, headers=request_config)


```