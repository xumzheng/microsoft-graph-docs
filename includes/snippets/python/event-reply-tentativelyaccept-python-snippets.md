---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TentativelyAcceptPostRequestBody()
request_body.comment = 'I will probably be able to make it.'

request_body.sendResponse = true



request_configuration = TentativelyAcceptRequestBuilderPostRequestConfiguration(
)


await client.me.events_by_id('event-id').tentativelyAccept.post(request_body = request_body)


```