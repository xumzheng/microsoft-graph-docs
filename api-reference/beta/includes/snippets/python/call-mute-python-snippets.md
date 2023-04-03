---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MutePostRequestBody();
requestBody.setClientContext('clientContext-value');



result = awaitclient.communications().callsById('call-id').mute().post(requestBody);


```