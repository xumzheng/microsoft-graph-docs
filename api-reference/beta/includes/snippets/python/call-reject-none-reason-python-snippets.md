---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = RejectPostRequestBody();
requestBody.setReason(RejectReason('none'));



await client.communications().callsById('call-id').reject().post(requestBody);


```