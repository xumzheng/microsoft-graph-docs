---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UsersRequestBuilderGetRequestConfiguration(
request_config = UsersRequestBuilderGetRequestConfiguration(query_params=query_params = UsersRequestBuilderGetQueryParameters()
query_params.count = true
query_params.select = ["id","displayName","customSecurityAttributes"]
query_params.filter = "customSecurityAttributes/Marketing/AppCountry eq 'Canada'"

)
query_params = UsersRequestBuilderGetQueryParameters()
query_params.count = true
query_params.select = ["id","displayName","customSecurityAttributes"]
query_params.filter = "customSecurityAttributes/Marketing/AppCountry eq 'Canada'"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.users.get(request_config, headers=request_config)


```