---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SetPresencePostRequestBody();
requestBody.setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87');

requestBody.setAvailability('Available');

requestBody.setActivity('Available');

$requestBody.setExpirationDuration( \DateInterval('PT1H'));



await client.usersById('user-id').presence().setPresence().post(requestBody);


```