---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = RejectPostRequestBody();
requestBody.setReason(RejectReason('none'));



graphServiceClient.communications().callsById('call-id').reject().post(requestBody);


```