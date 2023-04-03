---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Subscription();
requestBody.setChangeType('created,updated');

requestBody.setNotificationUrl('https://webhook.azurewebsites.net/notificationClient');

requestBody.setResource('/me/mailfolders(\'inbox\')/messages');

requestBody.setExpirationDateTime(DateTime('2016-03-20T11:00:00.0000000Z'));

requestBody.setClientState('SecretClientState');



result = await client.subscriptions().post(requestBody);


```