---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['filter'] = "MentionsPreview/IsMentioned eq true"
query_params['select'] = ["Subject","Sender","ReceivedDateTime","MentionsPreview"]

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['filter'] = "MentionsPreview/IsMentioned eq true"
query_params['select'] = ["Subject","Sender","ReceivedDateTime","MentionsPreview"]

)


result = await client.me.messages.get(request_configuration)


```