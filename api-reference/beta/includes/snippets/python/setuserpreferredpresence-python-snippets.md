---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SetUserPreferredPresencePostRequestBody();
requestBody.setAvailability('DoNotDisturb');

requestBody.setActivity('DoNotDisturb');

$requestBody.setExpirationDuration( \DateInterval('PT8H'));



await client.usersById('user-id').presence().setUserPreferredPresence().post(requestBody);


```