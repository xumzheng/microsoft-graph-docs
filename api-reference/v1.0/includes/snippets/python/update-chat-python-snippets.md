---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Chat()
request_body.setTopic('Group chat title update')



result = await client.chats_by_id('chat-id').patch(request_body)


```