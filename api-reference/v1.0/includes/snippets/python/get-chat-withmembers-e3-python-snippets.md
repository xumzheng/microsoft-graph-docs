---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ChatRequestBuilderGetRequestConfiguration(
request_configuration = ChatRequestBuilderGetRequestConfiguration(query_params=query_params = ChatRequestBuilderGetQueryParameters()
query_params['expand'] = ["members"]

)
query_params = ChatRequestBuilderGetQueryParameters()
query_params['expand'] = ["members"]

)


result = await client.chats_by_id('chat-id').get(request_configuration)


```