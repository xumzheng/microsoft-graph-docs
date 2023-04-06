---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UsersRequestBuilderGetRequestConfiguration(
request_configuration = UsersRequestBuilderGetRequestConfiguration(query_params=query_params = UsersRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","onPremisesExtensionAttributes"]

)
query_params = UsersRequestBuilderGetQueryParameters()
query_params['select'] = ["id","displayName","onPremisesExtensionAttributes"]

)


result = await client.users.get(request_configuration)


```