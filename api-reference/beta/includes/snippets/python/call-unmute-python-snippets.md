---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnmutePostRequestBody();
requestBody.setClientContext('clientContext-value');



result = awaitclient.communications().callsById('call-id').unmute().post(requestBody);


```