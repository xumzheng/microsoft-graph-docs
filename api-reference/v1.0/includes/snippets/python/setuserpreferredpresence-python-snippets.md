---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetUserPreferredPresencePostRequestBody()
request_body.setAvailability('DoNotDisturb')

request_body.setActivity('DoNotDisturb')

$request_body.setExpirationDuration( \DateInterval('PT8H'))



await client.usersby_id('user-id')_presence_setUserPreferredPresence.post(request_body)


```