---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration(
request_config = MessagesRequestBuilderGetRequestConfiguration(query_params=params['top'] = 2
params['filter'] = "lastModifiedDateTime gt 2021-03-17T07:13:28.000z"
params['orderby'] = ["createdDateTime desc"]
)


result = await client.users_by_id('user-id').chats_by_id('chat-id').messages.get(request_config, headers=request_config)


```