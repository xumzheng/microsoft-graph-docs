---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OnlineMeetingsRequestBuilderGetRequestConfiguration(
request_config = OnlineMeetingsRequestBuilderGetRequestConfiguration(query_params=query_params = OnlineMeetingsRequestBuilderGetQueryParameters()
query_params.filter = "VideoTeleconferenceId eq '123456789'"

)
query_params = OnlineMeetingsRequestBuilderGetQueryParameters()
query_params.filter = "VideoTeleconferenceId eq '123456789'"

)


result = await client.communications.onlineMeetings.get(request_config, headers=request_config)


```