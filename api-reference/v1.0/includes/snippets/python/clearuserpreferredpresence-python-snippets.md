---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClearUserPreferredPresencePostRequestBody()


await client.usersById('user-id').presence.clearUserPreferredPresence.post(request_body)


```