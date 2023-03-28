---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SetPresencePostRequestBody();
$requestBody.setSessionId('22553876-f5ab-4529-bffb-cfe50aa89f87');

$requestBody.setAvailability('Available');

$requestBody.setActivity('Available');

$requestBody.setExpirationDuration(new \DateInterval('PT1H'));



$graphServiceClient.usersById('user-id').presence().setPresence().post($requestBody);


```