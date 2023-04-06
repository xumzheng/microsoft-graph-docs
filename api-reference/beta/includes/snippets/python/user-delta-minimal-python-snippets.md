---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration(
request_config = DeltaRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["displayName","jobTitle","mobilePhone"]
)
headers['Prefer'] = "return=minimal"


result = await client.users.delta.get(request_config, headers=request_config)


```