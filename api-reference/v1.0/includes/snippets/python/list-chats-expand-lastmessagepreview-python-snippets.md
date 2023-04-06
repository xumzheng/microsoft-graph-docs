---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ChatsRequestBuilderGetRequestConfiguration(
request_config = ChatsRequestBuilderGetRequestConfiguration(query_params=query_params = ChatsRequestBuilderGetQueryParameters()
query_params.expand = ["lastMessagePreview"]

)
query_params = ChatsRequestBuilderGetQueryParameters()
query_params.expand = ["lastMessagePreview"]

)


result = await client.chats.get(request_config, headers=request_config)


```