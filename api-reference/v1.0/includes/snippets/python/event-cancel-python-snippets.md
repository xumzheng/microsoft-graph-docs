---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CancelPostRequestBody()
request_body.setComment('Cancelling for this week due to all hands')


request_config = CancelRequestBuilderPostRequestConfiguration(
request_config = CancelRequestBuilderPostRequestConfiguration(query_params=)


await client.me.events_by_id('event-id').cancel.post(request_body, headers=)


```