---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['filter'] = "Subject eq 'welcome' and importance eq 'normal'"
query_params['orderby'] = ["subject","importance","receivedDateTime desc"]

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['filter'] = "Subject eq 'welcome' and importance eq 'normal'"
query_params['orderby'] = ["subject","importance","receivedDateTime desc"]

)


result = await client.me.messages.get(request_configuration)


```