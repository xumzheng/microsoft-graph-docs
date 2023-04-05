---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RejectPostRequestBody()
request_body.setReason(RejectReason('none'))



await client.communications.calls_by_id('call-id').reject.post(request_body)


```