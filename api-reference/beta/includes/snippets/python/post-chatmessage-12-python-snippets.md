---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ChatMessage()
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('<emoji alt=\"😶‍🌫️\"></emoji>')


request_body.setBody($body)


result = await client.chatsById('chat-id').messages.post(request_body)


```