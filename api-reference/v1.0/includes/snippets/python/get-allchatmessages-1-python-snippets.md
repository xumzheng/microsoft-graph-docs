---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = MessagesRequestBuilder.MessagesRequestBuilderGetQueryParameters(
		top = 2,
)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.chats_by_id('chat-id').messages.get(request_configuration = request_configuration)


```