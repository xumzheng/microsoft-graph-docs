---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = MessagesRequestBuilder.MessagesRequestBuilderGetQueryParameters(
				top = 3,
)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.get(request_configuration = request_configuration)


```