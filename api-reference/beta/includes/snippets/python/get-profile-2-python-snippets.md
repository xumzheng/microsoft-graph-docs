---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ProfileRequestBuilderGetRequestConfiguration(
request_config = ProfileRequestBuilderGetRequestConfiguration(query_params=query_params = ProfileRequestBuilderGetQueryParameters()
query_params.expand = ["names($select=first,last)","skills($select=displayName)"]

)
query_params = ProfileRequestBuilderGetQueryParameters()
query_params.expand = ["names($select=first,last)","skills($select=displayName)"]

)


result = await client.me.profile.get(request_config, headers=request_config)


```