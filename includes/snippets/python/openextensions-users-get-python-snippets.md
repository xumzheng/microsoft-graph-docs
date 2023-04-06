---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MeRequestBuilderGetRequestConfiguration(
request_configuration = MeRequestBuilderGetRequestConfiguration(query_params=query_params = MeRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","mail","mobilePhone"]
query_params['expand'] = ["extensions"]

)
query_params = MeRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","mail","mobilePhone"]
query_params['expand'] = ["extensions"]

)


result = await client.me.get(request_configuration)


```