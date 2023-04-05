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
query_params.filter = "startsWith(customSecurityAttributes/Marketing/EmployeeId,'GS')"

headers = [
'ConsistencyLevel' => 'eventual',
]

)


result = await client.users.get(request_config)


```