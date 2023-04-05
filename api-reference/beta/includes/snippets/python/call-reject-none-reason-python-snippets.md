---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RejectPostRequestBody()
request_body.setReason(RejectReason('none'))



await client.communications_callsby_id('call-id')_reject.post(request_body)


```