---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration()

query_params = MessagesRequestBuilderGetQueryParameters()
query_params.filter = "Subject eq 'welcome' and importance eq 'normal'"
query_params.orderby = ["subject","importance","receivedDateTime desc"]

request_config.queryParameters = query_params


result = await client.me.messages.get(request_config)


```