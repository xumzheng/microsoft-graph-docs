---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SetUserPreferredPresencePostRequestBody();
$requestBody.setAvailability('DoNotDisturb');

$requestBody.setActivity('DoNotDisturb');

$requestBody.setExpirationDuration(new \DateInterval('PT8H'));



$graphServiceClient.usersById('user-id').presence().setUserPreferredPresence().post($requestBody);


```