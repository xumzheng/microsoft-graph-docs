---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UsersRequestBuilderGetRequestConfiguration(
query_params = UsersRequestBuilderGetQueryParameters()
query_params.count = true
query_params.select = ["id","displayName","customSecurityAttributes"]
query_params.filter = "customSecurityAttributes/Marketing/AppCountry eq 'Canada'"

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.users.get(request_config)


```