---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration()

query_params = GroupRequestBuilderGetQueryParameters()
query_params.count = true
query_params.orderby = ["displayName"]
query_params.filter = "startswith(displayName,%20'a')"

headers = [
'ConsistencyLevel' => 'eventual',
]

request_config.queryParameters = query_params
request_config.headers = headers


result = await client.devices._by_id('device-id').transitiveMemberOf.graphgroup.get(request_config)


```