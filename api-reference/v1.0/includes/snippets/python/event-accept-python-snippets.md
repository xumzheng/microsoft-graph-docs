---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AcceptPostRequestBody()
request_body.setComment('comment-value')

request_body.setSendResponse(true)



await client.me.events_by_id('event-id').accept.post(request_body)


```