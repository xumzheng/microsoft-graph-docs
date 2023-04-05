---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CancelPostRequestBody()
request_body.setComment('Cancelling for this week due to all hands')



await client.me.eventsById('event-id').cancel.post(request_body)


```