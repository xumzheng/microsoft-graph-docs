---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClearPresencePostRequestBody()
request_body.setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87')



await client.usersby_id('user-id').presence.clearPresence.post(request_body)


```