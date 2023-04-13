---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PinnedMessagesRequestBuilder.PinnedMessagesRequestBuilderGetQueryParameters(
		expand = ["message"],
)

request_configuration = PinnedMessagesRequestBuilder.PinnedMessagesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.chats_by_id('chat-id').pinnedMessages.get(request_configuration = request_configuration)


```