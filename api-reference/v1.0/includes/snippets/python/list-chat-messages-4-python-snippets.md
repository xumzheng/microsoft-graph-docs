---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration()

query_params = MessagesRequestBuilderGetQueryParameters()
query_params.top = 2
query_params.orderby = ["lastModifiedDateTime desc"]
query_params.filter = "lastModifiedDateTime gt 2022-09-22T00:00:00.000Z and lastModifiedDateTime lt 2022-09-24T00:00:00.000Z"

request_config.queryParameters = query_params


result = await client.chats._by_id('chat-id').messages.get(request_config)


```