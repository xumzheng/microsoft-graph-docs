---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MovePostRequestBody()
request_body.destinationId = 'deleteditems'




result = await client.me.messages_by_id('message-id').move.post(request_body = request_body)


```