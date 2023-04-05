---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
query_params = GroupsRequestBuilderGetQueryParameters()
query_params.filter = "createdDateTime ge 2021-11-01"
query_params.count = true

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.groups.get(request_config)


```