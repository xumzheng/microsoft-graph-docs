---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = GetAllMessagesRequestBuilder.GetAllMessagesRequestBuilderGetQueryParameters(
		top = 2,
)

request_configuration = GetAllMessagesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.users_by_id('user-id').chats.getAllMessages.get(request_configuration = request_configuration)


```