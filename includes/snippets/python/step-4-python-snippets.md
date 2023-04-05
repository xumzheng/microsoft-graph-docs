---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration(
query_params = MessagesRequestBuilderGetQueryParameters()
query_params.top = 2
query_params.filter = "lastModifiedDateTime gt 2021-03-17T07:13:28.000z"
query_params.orderby = ["createdDateTime desc"]

)


result = await client.users_by_id('user-id').chats_by_id('chat-id').messages.get(request_config)


```