---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['top'] = 3

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['top'] = 3

)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.get(request_configuration)


```