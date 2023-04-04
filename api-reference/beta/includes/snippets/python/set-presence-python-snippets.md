---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SetPresencePostRequestBody();
request_body.setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87');

request_body.setAvailability('Available');

request_body.setActivity('Available');

$request_body.setExpirationDuration( \DateInterval('PT1H'));



await client.usersById('user-id').presence.setPresence.post(request_body);


```