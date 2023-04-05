---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ChatRequestBuilderGetRequestConfiguration(
query_params = ChatRequestBuilderGetQueryParameters()
query_params.expand = ["lastMessagePreview"]

)


result = await client.chats_by_id('chat-id').get(request_config)


```