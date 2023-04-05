---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TentativelyAcceptPostRequestBody()
request_body.setComment('I will probably be able to make it.')

request_body.setSendResponse(true)



await client.me.events_by_id('event-id').tentativelyAccept.post(request_body)


```