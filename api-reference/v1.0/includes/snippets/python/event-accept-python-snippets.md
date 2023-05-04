---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Accept_post_request_body()
request_body.comment = 'comment-value'

request_body.send_response = True




await client.me.events.by_event_id('event-id').accept.post(request_body = request_body)


```