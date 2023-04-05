---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration()

query_params = MessagesRequestBuilderGetQueryParameters()
query_params.top = 2
query_params.orderby = ["createdDateTime desc"]

request_config.queryParameters = query_params


result = await client.chatsby_id('chat-id').messages.get(request_config)


```