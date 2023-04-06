---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessageRequestBuilderGetRequestConfiguration(
request_configuration = MessageRequestBuilderGetRequestConfiguration(query_params=query_params = MessageRequestBuilderGetQueryParameters()
query_params['select'] = ["internetMessageHeaders"]

)
query_params = MessageRequestBuilderGetQueryParameters()
query_params['select'] = ["internetMessageHeaders"]

)


result = await client.me.messages_by_id('message-id').get(request_configuration)


```