---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TentativelyAcceptPostRequestBody()
request_body.setComment('I will probably be able to make it.')

request_body.setSendResponse(true)



await client.me_eventsby_id('event-id')_tentativelyAccept.post(request_body)


```