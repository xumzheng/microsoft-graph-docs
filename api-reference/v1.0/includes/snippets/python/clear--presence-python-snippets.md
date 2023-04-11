---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClearPresencePostRequestBody()
request_body.sessionId = '22553876-f5ab-4529-bffb-cfe50aa89f87'



request_configuration = ClearPresenceRequestBuilderPostRequestConfiguration(
)


await client.users_by_id('user-id').presence.clearPresence.post(request_body = request_body)


```