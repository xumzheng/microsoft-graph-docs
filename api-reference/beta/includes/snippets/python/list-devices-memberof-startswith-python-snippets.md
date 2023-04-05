---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration(
query_params = GroupRequestBuilderGetQueryParameters()
query_params.count = true
query_params.orderby = ["displayName"]
query_params.filter = "startswith(displayName,%20'A')"

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.devices_by_id('device-id').memberOf.graphgroup.get(request_config)


```