---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MuteAllPostRequestBody();
requestBody.setParticipants(['', ]);

requestBody.setClientContext('clientContext-value');



result = awaitclient.communications().callsById('call-id').participants().muteAll().post(requestBody);


```