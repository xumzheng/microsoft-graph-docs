---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.setContent('Hello World')


request_body.setBody($body)


result = await client.teamsby_id('team-id').channelsby_id('channel-id').messages.post(request_body)


```