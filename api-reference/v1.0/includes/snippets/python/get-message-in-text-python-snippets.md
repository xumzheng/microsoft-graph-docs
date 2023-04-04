---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = MessageRequestBuilderGetRequestConfiguration()

query_params = MessageRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview","uniqueBody"]

headers = [
'Prefer' => 'outlook.body-content-type="text"',
]

request_config.queryParameters = query_params
request_config.headers = headers


result = await client.me.messagesById('message-id').get(request_config)


```