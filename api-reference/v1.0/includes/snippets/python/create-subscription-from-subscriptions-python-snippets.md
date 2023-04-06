---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Subscription()
request_body.setChangeType('created')

request_body.setNotificationUrl('https://webhook.azurewebsites.net/api/send/myNotifyClient')

request_body.setResource('me/mailFolders(\'Inbox\')/messages')

request_body.setExpirationDateTime(DateTime('2016-11-20T18:23:45.9356913Z'))

request_body.setClientState('secretClientValue')

request_body.setLatestSupportedTlsVersion('v1_2')



result = await client.subscriptions.post(request_body, headers=)


```