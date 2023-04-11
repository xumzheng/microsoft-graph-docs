---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetUserPreferredPresencePostRequestBody()
request_body.availability = 'DoNotDisturb'

request_body.activity = 'DoNotDisturb'

request_body.expirationduration =  \DateInterval('PT8H')



request_configuration = SetUserPreferredPresenceRequestBuilderPostRequestConfiguration(
)


await client.users_by_id('user-id').presence.setUserPreferredPresence.post(request_body = request_body)


```