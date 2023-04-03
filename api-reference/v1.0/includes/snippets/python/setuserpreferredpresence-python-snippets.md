---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SetUserPreferredPresencePostRequestBody();
requestBody.setAvailability('DoNotDisturb');

requestBody.setActivity('DoNotDisturb');

$requestBody.setExpirationDuration( \DateInterval('PT8H'));



awaitclient.usersById('user-id').presence().setUserPreferredPresence().post(requestBody);


```