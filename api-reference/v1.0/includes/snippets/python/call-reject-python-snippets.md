---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RejectPostRequestBody()
request_body.setReason(RejectReason('busy'))


request_config = RejectRequestBuilderPostRequestConfiguration(
request_config = RejectRequestBuilderPostRequestConfiguration(query_params=)


await client.communications.calls_by_id('call-id').reject.post(request_body, headers=)


```