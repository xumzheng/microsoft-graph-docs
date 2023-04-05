---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GetAllMessagesRequestBuilderGetRequestConfiguration()

query_params = GetAllMessagesRequestBuilderGetQueryParameters()
query_params.top = 2

request_config.queryParameters = query_params


result = await client.users_by_id('user-id').chats.getAllMessages.get(request_config)


```