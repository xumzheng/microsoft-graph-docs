---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserRequestBuilderGetRequestConfiguration(
request_config = UserRequestBuilderGetRequestConfiguration(query_params=query_params = UserRequestBuilderGetQueryParameters()
query_params.count = true
query_params.orderby = ["displayName"]
query_params.search = "\"displayName:tier\""
query_params.select = ["displayName","id"]

)
query_params = UserRequestBuilderGetQueryParameters()
query_params.count = true
query_params.orderby = ["displayName"]
query_params.search = "\"displayName:tier\""
query_params.select = ["displayName","id"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups_by_id('group-id').transitiveMembers.graphuser.get(request_config, headers=request_config)


```