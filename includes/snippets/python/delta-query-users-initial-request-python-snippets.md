---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = DeltaRequestBuilderGetRequestConfiguration(
request_configuration = DeltaRequestBuilderGetRequestConfiguration(query_params=query_params = DeltaRequestBuilderGetQueryParameters()
query_params['select'] = ["displayName","givenName","surname"]

)
query_params = DeltaRequestBuilderGetQueryParameters()
query_params['select'] = ["displayName","givenName","surname"]

)


result = await client.users.delta.get(request_configuration)


```