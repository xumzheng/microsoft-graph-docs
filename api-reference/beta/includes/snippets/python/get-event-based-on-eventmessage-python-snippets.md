---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessageRequestBuilderGetRequestConfiguration()

query_params = MessageRequestBuilderGetQueryParameters()
query_params.expand = ["microsoft.graph.eventMessage/event"]

request_config.queryParameters = query_params


result = await client.me.messages_by_id('message-id').get(request_config)


```