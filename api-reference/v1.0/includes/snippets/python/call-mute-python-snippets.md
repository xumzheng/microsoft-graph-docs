---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = MutePostRequestBody();
requestBody.setClientContext('clientContext-value');



requestResult = graphServiceClient.communications().callsById('call-id').mute().post(requestBody);


```