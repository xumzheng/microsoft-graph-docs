---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnmutePostRequestBody()
request_body.setClientContext('clientContext-value')



result = await client.communications.callsById('call-id').unmute.post(request_body)


```