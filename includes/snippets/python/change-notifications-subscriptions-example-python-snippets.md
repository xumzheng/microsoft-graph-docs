---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Subscription();
$requestBody->setChangeType('created,updated');

$requestBody->setNotificationUrl('https://webhook.azurewebsites.net/notificationClient');

$requestBody->setResource('/me/mailfolders(\'inbox\')/messages');

$requestBody->setExpirationDateTime(new DateTime('2016-03-20T11:00:00.0000000Z'));

$requestBody->setClientState('SecretClientState');



$requestResult = $graphServiceClient->subscriptions()->post($requestBody);


```