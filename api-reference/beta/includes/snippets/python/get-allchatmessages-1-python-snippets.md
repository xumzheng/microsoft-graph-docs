---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['top'] = 2
query_params['orderby'] = ["createdDateTime desc"]

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['top'] = 2
query_params['orderby'] = ["createdDateTime desc"]

)


result = await client.chats_by_id('chat-id').messages.get(request_configuration)


```