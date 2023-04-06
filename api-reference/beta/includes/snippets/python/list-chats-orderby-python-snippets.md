---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ChatsRequestBuilderGetRequestConfiguration(
request_configuration = ChatsRequestBuilderGetRequestConfiguration(query_params=query_params = ChatsRequestBuilderGetQueryParameters()
query_params['orderby'] = ["lastMessagePreview/createdDateTime desc"]

)
query_params = ChatsRequestBuilderGetQueryParameters()
query_params['orderby'] = ["lastMessagePreview/createdDateTime desc"]

)


result = await client.chats.get(request_configuration)


```