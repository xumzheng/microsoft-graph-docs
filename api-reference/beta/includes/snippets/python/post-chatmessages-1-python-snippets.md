---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.setContent('Hello world')


request_body.setBody($body)

request_config = MessagesRequestBuilderPostRequestConfiguration(
request_config = MessagesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.chats_by_id('chat-id').messages.post(request_body, headers=)


```