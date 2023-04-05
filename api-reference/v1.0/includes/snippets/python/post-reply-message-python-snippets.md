---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('Hello World')


request_body.setBody($body)


result = await client.teamsby_id('team-id')_channelsby_id('channel-id')_messagesby_id('chatMessage-id')_replies.post(request_body)


```