---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnmutePostRequestBody();
requestBody.setClientContext('clientContext-value');



result = await client.communications().callsById('call-id').unmute().post(requestBody);


```