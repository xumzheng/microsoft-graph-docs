---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PinnedMessagesRequestBuilderGetRequestConfiguration(
query_params = PinnedMessagesRequestBuilderGetQueryParameters()
query_params.expand = ["message"]

)


result = await client.chats_by_id('chat-id').pinnedMessages.get(request_config)


```