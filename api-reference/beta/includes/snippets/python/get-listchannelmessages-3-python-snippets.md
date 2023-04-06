---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration(
request_config = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params.top = 1
query_params.expand = ["replies"]

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params.top = 1
query_params.expand = ["replies"]

)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.get(request_config, headers=request_config)


```