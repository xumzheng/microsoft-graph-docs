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


result = await client.teams._by_id('team-id').channels._by_id('channel-id').messages._by_id('chatMessage-id').replies.post(request_body)


```