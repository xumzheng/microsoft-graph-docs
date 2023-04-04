---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Subscription()
request_body.setChangeType('created,updated')

request_body.setNotificationUrl('https://webhook.azurewebsites.net/notificationClient')

request_body.setResource('/me/mailfolders(\'inbox\')/messages')

request_body.setExpirationDateTime(DateTime('2016-03-20T11:00:00.0000000Z'))

request_body.setClientState('SecretClientState')



result = await client.subscriptions.post(request_body)


```