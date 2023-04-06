---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['top'] = 2
query_params['orderby'] = ["lastModifiedDateTime desc"]
query_params['filter'] = "lastModifiedDateTime gt 2022-09-22T00:00:00.000Z and lastModifiedDateTime lt 2022-09-24T00:00:00.000Z"

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['top'] = 2
query_params['orderby'] = ["lastModifiedDateTime desc"]
query_params['filter'] = "lastModifiedDateTime gt 2022-09-22T00:00:00.000Z and lastModifiedDateTime lt 2022-09-24T00:00:00.000Z"

)


result = await client.chats_by_id('chat-id').messages.get(request_configuration)


```