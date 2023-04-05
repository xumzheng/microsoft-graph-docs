---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserRequestBuilderGetRequestConfiguration(
query_params = UserRequestBuilderGetQueryParameters()
query_params.count = true
query_params.orderby = ["displayName"]
query_params.search = "\"displayName:Pr\""
query_params.select = ["displayName","id"]

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.groups_by_id('group-id').members.graphuser.get(request_config)


```